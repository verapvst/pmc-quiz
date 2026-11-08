# PMC Live Quiz: guia rápido

Link do quiz (para os participantes): https://verapvst.github.io/pmc-quiz/
Painel de controlo (para ti e para o teu pai): https://verapvst.github.io/pmc-quiz/?host=bpi

## Como funciona

No painel de controlo tens tudo num sítio:
1. Respostas: quantas já responderam, botão para adicionar 50 respostas de teste, botão para as remover, e o botão Restart quiz que apaga todas as respostas.
2. Apresentação: o teu pai carrega aqui o PDF dele.
3. Guest outlier: a pontuação do teu pai (por defeito 3) e o texto (por defeito "Me at your age").
4. Live preview: vês a curva a crescer, com a barra do teu pai a cinzento.
5. Botão Present: arranca a apresentação em ecrã inteiro.

Quando carregas em Present, a ordem é:
1. QR code, com o contador de quem já respondeu.
2. Resultados ao vivo. A pontuação do teu pai aparece como mais uma barra, a cinzento, em cima da barra da sala.
3. O mesmo ecrã: a barra dele fica laranja e aparece uma seta com o texto "Me at your age".
4. Os slides do PDF que ele carregou.

## Navegar na apresentação

Espaço, seta direita, PageDown ou Enter avançam. Seta esquerda, PageUp ou Backspace recuam. F liga e desliga o ecrã inteiro. Esc volta ao painel. A barra de botões no canto de baixo desaparece sozinha e volta quando mexes no rato. O comando de apresentação (clicker) funciona se enviar PageUp e PageDown.

## Carregar o PDF

1. No PowerPoint: Ficheiro, Exportar, Criar PDF (ou Guardar como PDF).
2. No painel, em Presentation, carrega em Upload PDF e escolhe o ficheiro.
3. Espera pela barra de progresso. No fim aparece "Done" e o nome do ficheiro.

Um PowerPoint (.pptx) não pode ser lido diretamente pelo browser, por isso tem de ir em PDF. Cada slide é guardado como imagem, por isso animações e vídeos não funcionam, só o aspeto final de cada slide. Prefere PDFs com menos de 40 slides.

## Teste e dia do evento

Agora: usa "Add 50 mock answers" para veres a curva e carrega em Present para ensaiar a sequência. Podes também responder tu ao quiz no telemóvel.

No dia: carrega em Restart quiz (pede dois cliques) para apagar tudo, incluindo respostas de teste. O PDF e a pontuação do teu pai ficam guardados. Confirma que o contador mostra 0 antes de começar.

## Notas

1. A base de dados está em modo de teste, aberta a quem tiver o link, e fecha sozinha a 8 de dezembro de 2026. Depois do evento podes apagar o projeto no Firebase.
2. Não há nomes. Cada pessoa só vê a própria pontuação e a curva da sala.
3. Se mudares o index.html, volta a carregá-lo no repositório do GitHub (Add file, Upload files, substituir) e espera 1 a 2 minutos.
4. Testa tudo no computador e no projetor da sala antes do comité.
