# Sonar ABI

Detector de possibilidades de itens do mercador em Arena Breakout Infinite pelo som de pickup. Compartilhe a tela do jogo com o áudio do sistema, pegue um item e use as pistas de tamanho e cor para filtrar a lista.

## Publicar no GitHub Pages

O site está inteiro em `index.html`; não precisa de instalação, build ou servidor próprio. Nas configurações do repositório, em **Pages**, selecione **Deploy from a branch**, a branch principal e a pasta **/ (root)**. Abra o endereço HTTPS informado pelo GitHub após a publicação.

Para usar a captura, abra o site no Chrome ou Edge, clique em **Compartilhar jogo** e marque **Compartilhar áudio do sistema** no seletor do navegador. A página analisa o áudio localmente; não envia áudio nem imagem. O vídeo compartilhado não é analisado: tamanho e cor são selecionados manualmente.

O detector atual tem 22 sons, 3.208 itens relacionados a eles e ícones para 1.179 itens. O resultado mostra possibilidades, não uma identificação garantida. Outros eventos de pickup ainda não estão incluídos.

O CSS do [Basecoat UI](https://basecoatui.com/) e a fonte Geist Sans estão incorporados no HTML. As licenças correspondentes estão em `third_party/`.
