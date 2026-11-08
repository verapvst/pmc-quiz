# PMC Live Quiz: guia rápido

Link do quiz (para os participantes): https://verapvst.github.io/pmc-quiz/
Painel de controlo (para ti e para o teu pai): https://verapvst.github.io/pmc-quiz/?host=bpi

## O quiz

No telemóvel cada pergunta ocupa o ecrã todo: toca em Yes ou No, passa sozinho para a seguinte com uma animação, e há uma seta para voltar atrás. A barra de progresso fica no topo.

Título: "How’s your portfolio of experiences?". São 13 perguntas (12 de sim ou não, "Have you...", mais uma sobre instrumentos financeiros), no máximo 17 pontos. No fim cada pessoa vê "Your return" (a sua pontuação), o "Benchmark" (média da sala), a frase "You outperformed X% of the room." e o gráfico da sala.

## Separador Quiz

No painel há dois separadores: Control room e Quiz. No separador Quiz o teu pai pode editar o título e o subtítulo, a frase do slide do QR (o {n} vira o número de perguntas), as perguntas de sim ou não (escrever, acrescentar, apagar com dois cliques, arrastar pelo ícone dos pontos ou usar as setas) e a pergunta dos instrumentos (título, opções, ordem). À direita há uma pré-visualização do telemóvel que acompanha o que ele está a editar. As alterações guardam sozinhas e chegam logo aos telemóveis. O topo da pontuação ajusta-se ao número de perguntas. Se já houver respostas, aparece um aviso: depois de editar, faz Restart quiz. O botão "Reset to the original questions" volta às perguntas iniciais.

## Separador Slides

O terceiro separador deixa o teu pai editar as palavras dos três slides do quiz: o do QR code (linha pequena, título, linha por baixo e o texto ao lado do contador), e os dois dos resultados (título de cada um e a linha pequena à direita, onde {count}, {avg} e {max} são preenchidos ao vivo). À direita há uma pré-visualização do slide, com setas para ver os três. A pontuação do teu pai (por defeito 1) e o texto da seta ("Me at your age") também estão aqui, no cartão Guest, e a pré-visualização mostra a seta ao vivo. Os slides do PDF vêm depois destes três.

## Painel de controlo (separador Control room)

Três cartões numerados:
1. Presentation: o teu pai carrega aqui o PDF (clicar ou arrastar).
2. Test with mock answers: simula 50 pessoas a responder, uma a uma ao longo de cerca de 15 segundos (podes carregar em Stop simulation), e remove-as. Para ensaiar a animação: remove as respostas, carrega em Add 50 mock answers e logo a seguir em Present. Adiciona respostas de teste (a média fica mais à direita, como num clube de gestão de carteiras) e remove-as.
3. On the day: botão Restart quiz, que apaga todas as respostas.

Há ainda o botão Present e o link dos participantes com um QR pequeno. A caixa "Before the event" mostra três verificações: carregar a apresentação (opcional), apagar as respostas de teste e reiniciar o quiz. Quando tudo está feito aparece "Ready for the day". Podes apresentar mesmo sem PDF.

## Ordem da apresentação (botão Present)

1. QR code ("Beat the benchmark. 13 questions, 2 minutes.") com o contador de quem já respondeu.
2. Resultados ao vivo, barras a cinzento. A pontuação do teu pai já está incluída, mas ainda não se vê qual é.
3. O mesmo gráfico, sem mudar de forma. Aparece a seta "Me at your age" e a parte da barra do teu pai fica laranja.
4. Os slides do PDF.

O logo do BPI aparece no canto de baixo à direita.

## Navegar

Espaço, seta direita, PageDown ou Enter avançam. Seta esquerda, PageUp ou Backspace recuam. F liga e desliga o ecrã inteiro. Esc volta ao painel. A barra de botões desaparece sozinha e volta quando mexes no rato. Um clicker que envie PageUp e PageDown funciona.

## Carregar o PDF

1. No PowerPoint: Ficheiro, Exportar, Criar PDF.
2. No painel, em Presentation, carrega o ficheiro.
3. Espera pela barra de progresso até aparecer "Done".

Um .pptx não pode ser lido pelo browser, por isso tem de ir em PDF. Cada slide fica como imagem, por isso animações e vídeos não funcionam. Prefere PDFs com menos de 40 slides.

## Antes do dia

1. Carrega um PDF a sério e confirma que os slides aparecem (isto ainda não foi testado num browser real).
2. Usa as respostas de teste e ensaia a sequência toda em Present.
3. Responde ao quiz no telemóvel e confirma que o QR abre a página certa.
4. No dia: apaga as respostas de teste, carrega em Restart quiz (dois cliques) e confirma que o contador mostra 0.

## Notas

1. A base de dados está em modo de teste, aberta a quem tiver o link, e fecha sozinha a 8 de dezembro de 2026. Depois do evento podes apagar o projeto no Firebase.
2. Não há nomes. Cada pessoa só vê a própria pontuação e a curva da sala.
3. Se mudares o index.html, volta a carregá-lo no GitHub (Add file, Upload files, substituir) e espera 1 a 2 minutos.
4. Testa tudo no computador e no projetor da sala antes do comité.
