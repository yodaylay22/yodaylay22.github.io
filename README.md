# Sonar ABI

Detector de possibilidades de itens do mercador em Arena Breakout Infinite pelo som de pickup. Compartilhe a tela do jogo com o áudio do sistema, pegue um item e use as pistas de tamanho e cor para filtrar a lista.

## Publicar no GitHub Pages

O site está inteiro em `index.html`; não precisa de instalação, build ou servidor próprio. Nas configurações do repositório, em **Pages**, selecione **Deploy from a branch**, a branch principal e a pasta **/ (root)**. Abra o endereço HTTPS informado pelo GitHub após a publicação.

Para usar a captura, abra o site no Chrome ou Edge, clique em **Compartilhar jogo** e marque **Compartilhar áudio do sistema** no seletor do navegador. A página analisa o áudio localmente; não envia áudio nem imagem. O vídeo compartilhado não é analisado: tamanho e cor são selecionados manualmente.

O detector atual está focado em itens vermelhos diversos que podem aparecer em cofres. Ele tem 10 sons e 42 candidatos, todos com ícones. Munição, cartões, cosméticos e itens de evento ficam fora. O filtro combina a categoria e os campos de saque do jogo com as marcações manuais recebidas; ele é uma inferência e ainda pode precisar de correções. O resultado mostra possibilidades, não uma identificação garantida. Outros eventos de pickup ainda não estão incluídos.

A sensibilidade inicial é 60%. Esse valor representa a semelhança mínima exigida para reconhecer um som: reduzi-lo encontra mais sons, mas aumenta os enganos; aumentá-lo pode deixar passar pickups com ruído. O detector compara o áudio com os sons de pegar e de soltar: descarta retornos de item e tenta identificar um pickup mesmo quando outro efeito toca junto. A confirmação pode demorar um pouco mais nos sons parecidos.

A faixa de quadrados registra trechos de áudio acima de um volume mínimo, no máximo uma vez por segundo: cinza quando não há identificação e verde quando um pickup é reconhecido. O resultado atual mostra há quanto tempo foi identificado.

A página abre em 🇺🇸 English para novos visitantes e também oferece 🇧🇷 Português (BR). A escolha de idioma e a sensibilidade alterada ficam salvas em cookies no GitHub Pages, com armazenamento local como apoio para o HTML aberto diretamente no computador. A **Wiki de sons** reúne os 10 pickups e os 42 itens vermelhos aprovados, com áudio, ícone, nome e tamanho.


