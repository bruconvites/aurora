# Convite da Aurora — como publicar no GitHub Pages

## O que tem aqui
- `index.html` — a página do convite (é só isso que faz tudo funcionar)
- `assets/` — as suas imagens, vídeos e a música

## Fluxo que já está programado
1. Abre em `primeira.jpg` → clique em qualquer lugar da tela → toca a música de fundo e vai para `video1.mp4`
2. `video1` → `video2` → ... → `video8` (avança sozinho quando cada vídeo termina)
3. Depois do `video8` → vai para `ultima.jpg`
4. Em `ultima.jpg`: tocar no selo "Confirme presença" abre o WhatsApp; tocar no selo "Localização" abre o Google Maps
5. Durante os vídeos aparece um botãozinho dourado "Clique aqui para avançar", que pula direto para `ultima.jpg`
6. Em `ultima.jpg` aparece um botãozinho dourado "Voltar ao convite", que volta para o `video1`
7. A cada toque na tela, em qualquer página, aparece uma coroinha dourada
8. Entre uma cena e outra tem uma transição de fumacinha rosa
9. Tem um botãozinho "♪" no canto para a pessoa silenciar a música, se quiser

## Importante sobre os nomes dos arquivos
O código espera exatamente estes nomes dentro da pasta `assets/`:
```
primeira.jpg
video1.mp4
video2.mp4
video3.mp4
video4.mp4
video5.mp4
video6.mp4
video7.mp4
video8.mp4
ultima.jpg
audio.mp3
```
Troquei o `primeira.jpg` e os `videoN.mp4` que vieram do seu zip (que tinham nomes um pouco diferentes, como acento em "vídeo1.mp4") por essa versão sem acento e sem espaço — isso é necessário porque acentos e espaços em nomes de arquivo podem quebrar o link quando hospedado no GitHub Pages. Quando você tiver o `primeira.jpg` definitivo, é só substituir o arquivo dentro de `assets/` mantendo esse mesmo nome.

## Como publicar no GitHub Pages
1. Crie um repositório novo no GitHub (pode ser público ou privado, mas para o link funcionar sem login precisa ser público)
2. Suba todo o conteúdo desta pasta (o `index.html` e a pasta `assets/` inteira) para a raiz do repositório
3. Vá em **Settings → Pages**
4. Em "Source", selecione a branch (geralmente `main`) e a pasta `/root`
5. Salve — o GitHub vai te dar um link parecido com `https://seu-usuario.github.io/nome-do-repositorio/`
6. Esse é o link que você vai mandar para os convidados

Obs.: os vídeos deixam o repositório com uns 40 MB no total — dentro do limite do GitHub, sem problema.
