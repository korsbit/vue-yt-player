### Apresentação
---
VueYtPlayer é um player de vídeo baseado no player do youtube. Trata-se de um pequeno projeto desenvolvido como parte de um outro projeto maior, mas que ainda encontra-se em estado de desenvolvimento.

### Instalação
1. Clone o repositório
    ~~~
    https://github.com/korsbit/vue-yt-player.git
    ~~~
2. gora, já dentro do repositório, instale os pacotes com o npm
    ~~~
    npm install
    ~~~

[HTML5.io]: https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white
[CSS3.io]: https://img.shields.io/badge/css3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white
[Typescript.io]: https://img.shields.io/badge/typescript-%23007ACC.svg?style=for-the-badge&logo=typescript&logoColor=white

[Vue-url]: https://vuejs.org/
[Vue.io]: https://img.shields.io/badge/vuejs-%2335495e.svg?style=for-the-badge&logo=vuedotjs&logoColor=%234FC08D

### Manual de uso
O player vem no formato de componente e possui dois parâmetros:
- src ({qualidade: {src: caminho_do_video, origin_app: origem_do_video}}): informação sobre o vídeo a ser reproduzido
- width (string): largura do player

Obs: 'app_origin' é verdadeiro caso a origem do vídeo seja de dentro do próprio vue-yt-player, como no caso de um vídeo que esteja em '/assets' por exemplo.

#### Exemplos
~~~html
<yt-player :src="{ 1080: { src: 'assets/videos/elliot1_1080p.webm', app_origin: true }, 240: { src: 'assets/videos/elliot1_240p.webm', app_origin: true } }" width="60rem"/>
~~~
resultado:
    <img src="https://github.com/korsbit/vue-yt-player/blob/main/screenshots/screen1.png"/>

Obs: Para que o efeito cinematográfico funcione corretamente, o player de vídeo deve estar em cima de um elemento de cores escuras, de preferência #0F0F0F.

## Criado com

* [![HTML5][HTML5.io]][HTML5.io]
* [![CSS3][CSS3.io]][CSS3.io]
* [![Typescript][Typescript.io]][Typescript.io]
* [![Vue][Vue.io]][Vue-url]