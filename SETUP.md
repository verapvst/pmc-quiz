# PMC Live Quiz: como pôr a funcionar

Fluxo: o slide mostra o QR, cada pessoa responde a tudo no telemóvel em 2 ou 3 minutos, e o ecrã mostra a curva a crescer ao vivo, com o ponto do teu pai quando quiseres.

Tempo de preparação: cerca de 15 minutos. Só precisas de uma conta Google.

## 1. Criar a base de dados (Firebase, gratuito)

1. Abre console.firebase.google.com e entra com a tua conta Google.
2. Clica em "Create a project", escolhe um nome (por exemplo pmc quiz) e podes desligar o Google Analytics.
3. No menu da esquerda, vai a Build, depois Realtime Database, e clica em "Create Database".
4. Escolhe a localização Europe (Belgium) e começa em "test mode".
5. No separador Rules, confirma que está assim e clica em Publish:

```
{ "rules": { ".read": true, ".write": true } }
```

## 2. Copiar as credenciais

1. Na roda dentada, abre "Project settings", desce até "Your apps" e clica no ícone web (</>).
2. Dá um nome à app e regista. Aparece um bloco chamado firebaseConfig.
3. Se faltar o campo databaseURL, copia o endereço que aparece no topo da página do Realtime Database (começa por https:// e acaba em firebasedatabase.app).

## 3. Colar no ficheiro

(Já feito no ficheiro que te enviei: o projeto pmc-live-quiz está criado e as credenciais já estão coladas. Podes saltar as secções 1 a 3.)

1. Abre o index.html num editor de texto (Bloco de Notas serve).
2. No topo, no bloco FIREBASE_CONFIG, cola os valores entre as aspas.
3. Se quiseres, muda o HOST_PIN (a palavra que abre o ecrã de apresentador). Por defeito é bpi.

## 4. Pôr online

Netlify: cria uma pasta chamada quiz com o index.html lá dentro, abre app.netlify.com/drop, cria uma conta gratuita e arrasta a pasta.

GitHub: cria um repositório público, usa "Add file" e "Upload files" para carregar o index.html, depois vai a Settings, Pages, "Deploy from a branch", escolhe main e a pasta root.

Em ambos recebes um link. Os participantes usam o link normal. O apresentador usa o link seguido de /?host=bpi.

## 5. Ensaio (faz isto antes do comité)

1. Abre o link do apresentador no computador e o link normal no telemóvel.
2. No apresentador, abre "Rehearsal tools" e clica em "Add 50 test players".
3. Muda para "Curve view", depois carrega em "Reveal outlier" para ver o ponto do teu pai.
4. Responde tu ao quiz no telemóvel e vê a tua barra destacada.
5. No fim, "Remove test players" e "Reset quiz" deixam tudo limpo.

## 6. No dia

1. Slide 1 do PowerPoint: tira uma captura de ecrã ao QR code que aparece na "QR view" do apresentador e cola no slide. Podes também mostrar essa vista diretamente.
2. Deixa o ecrã de apresentador aberto num separador do browser, em ecrã inteiro (F11).
3. Enquanto as pessoas respondem, a "QR view" mostra quantas já responderam. Quando quiseres mostrar a curva, carrega no espaço (ou em "Curve view").
4. Quando o teu pai entrar, carrega em O (ou em "Reveal outlier"). Define a pontuação e o texto antes, na barra de baixo.
5. Atalhos: espaço troca entre QR e curva, O mostra ou esconde o outlier, H esconde os controlos. Os comandos de apresentação (PageUp e PageDown) também trocam a vista.

## 7. Opcional: slides ao vivo dentro do PowerPoint

Dá para ter o QR e a curva dentro do próprio PowerPoint, com um add-in que mostra uma página web viva num slide (por exemplo o LiveWeb, que pelo que sei só funciona no PowerPoint para Windows). O add-in tem de estar instalado no computador que vai apresentar, e a sala precisa de internet.

Use estes três endereços (troca o link pelo teu):
1. Slide do QR ao vivo: o teu link seguido de /?host=bpi&show=qr
2. Slide da curva ao vivo: o teu link seguido de /?host=bpi&show=curve
3. Comando à distância, no teu telemóvel: o teu link seguido de /?host=bpi

Nas páginas com show=qr e show=curve não aparecem botões. O ponto do teu pai é revelado pelo botão "Reveal outlier" no comando do teu telemóvel, e aparece logo no slide da curva.

Plano B se o add-in falhar: não uses o add-in, mostra a página show=curve num separador do browser e muda para ele com Alt+Tab no momento da curva.

Testa isto no computador da sala, com o projetor e o Wi-Fi de lá, antes do comité.

## 8. Modo apresentação: tudo no mesmo sítio (sem PowerPoint)

Em vez de saltar entre o PowerPoint e o browser, podes apresentar tudo a partir da página. O link é o teu seguido de /?host=bpi&deck=1

Por defeito tem dois slides: o QR e a curva ao vivo. Os slides do teu pai entram como imagens.

Como juntar os slides dele (quando os tiveres):
1. No PowerPoint: Ficheiro, Exportar, Alterar Tipo de Ficheiro, PNG, "Todos os Diapositivos". Dá uma pasta com imagens.
2. Ao lado do index.html cria uma pasta chamada slides e põe lá as imagens, com nomes simples (slide-01.png, slide-02.png, e assim por diante).
3. No index.html, procura SLIDES e acrescenta uma linha por imagem, na ordem em que queres. Exemplo:

```
const SLIDES = [
  { type: "qr" },
  { type: "curve" },
  { type: "image", src: "slides/slide-02.png" },
  { type: "image", src: "slides/slide-03.png" }
];
```

4. Faz upload outra vez (Netlify: arrasta a pasta quiz inteira, com index.html e slides).

Atalhos neste modo: espaço, seta direita, PageDown ou Enter avançam. Seta esquerda, PageUp ou Backspace recuam. O mostra ou esconde o ponto do teu pai, F ecrã inteiro, H esconde os controlos. O clicker normal do PowerPoint funciona se enviar PageUp e PageDown.

Ao voltar ao slide do QR, o ponto do teu pai desaparece sozinho, para o ensaio e o evento começarem limpos.

Se o pai não tiver o PowerPoint a tempo, usa só os dois slides ao vivo e mostra o resto no PowerPoint dele com Alt+Tab.

Estilo: as cores e tipografia seguem a apresentação do BPI que indicaste (fundo branco, laranja forte, títulos em maiúsculas com barra laranja, cinzento nos subtítulos). O logótipo da BPI Gestão de Ativos está embebido no próprio ficheiro, no topo de cada ecrã.

## Notas

1. O ponto do teu pai é um marcador à parte, não entra na contagem das pessoas.
2. Não há nomes nem nicknames. Cada pessoa só vê a própria pontuação e a curva da sala.
3. A segurança é simples e serve para um evento de uma noite. Depois do comité, apaga o projeto no Firebase.
