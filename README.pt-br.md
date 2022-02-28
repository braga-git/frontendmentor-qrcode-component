# Frontend Mentor - Solução do desafio "QR code component"

E aí! :call_me_hand:	

Essa é a minha solução para o [desafio "QR code component" do Frontend Mentor](https://www.frontendmentor.io/challenges/qr-code-component-iux_sIO_H). 

Os desafios do **Frontend Mentor** te ajudam a desenvolver suas habilidades de programação construindo projetos realistas. 

Read this in poor [English](README.md) :joy:	

## Índice

- [Visão geral](#visão-geral)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [Meu processo](#meu-processo)
  - [Criado com](#criado-com)
  - [O que aprendi](#o-que-aprendi)
  - [Para me aprofundar](#para-me-aprofundar)
  - [Recursos úteis](#recursos-úteis)
- [Autor](#autor)
- [Reconhecimentos](#reconhecimentos)

## Visão geral

### Screenshot

![Minha solução](https://github.com/braga-git/frontendmentor-qrcode-component/blob/main/design/mydesktop-design.png)

### Links

- [Arquivos da solução](https://github.com/braga-git/frontendmentor-qrcode-component)
- [Site](https://braga-git.github.io/frontendmentor-qrcode-component/)

## Meu processo

### Criado com

- HTML5
- CSS3

### O que aprendi

Como sou novo nesse mundo e acabei de começar a aprender HTML e CSS, a parte mais difícil pra eu fazer sozinho foi saber por onde começar. :sweat_smile:	

Ao meu ver, esse desafio é mais um desafio de CSS do que de HTML5. Minhas maiores dificuldades foram a respeito dos alinhamentos e interações entre `<img>` e `<div>`, pois as vezes eu estava tentando tentando configurar o padding da div e a imagem pulava para fora dela.

Isso foi muito fácil de resolver, eu simplesmente usei a propriedade `overflow` com o valor `hidden`:

```css
div.window-qr {
  overflow: hidden;
} 
```

Esse código esconderá o conteúdo que exceda a div.

Eu corrigi o problema da imagem saindo da div, mas ela ainda não estava centralizada. Ela deixava uma margem na esquerda e aparecia mais alta do que eu gostaria. Para resolver isso eu defini a largura da imagem `img width` para `100%`. 

```css
.window-qr img {
        width: 100%;
}
```

Isso fez com que a imagem ocupasse somente a largura da div. 

O último problema que eu tinha para resolver era como centralizar tanto horizontalmente quanto verticalmente o meu conteúdo. Dessa vez eu realmente não sabia o que fazer, mas pesquisei e encontrei uma forma que funcionou. Eu utilizei a propriedade `transform` com o valor `translate`:

```css
main {
    position: fixed;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
}
```

E eu não sei exatamente como esse código funciona, mas..

Em resumo, acredito que eu tenha lidado muito bem com o desafio. Bom, mesmo que o código não seja o melhor, o visual ficou bem parecido! :rofl:				

### Para me aprofundar

Eu vou continuar dando pesquisando maneiras de centralizar as coisas de forma correta pois, como eu disse, eu não sei 100% a usabilidade e função da propriedade `transform`. **Mas sei que não é o correto usar um código sem saber como ele funciona**. :man_shrugging:

### Recursos úteis

- [Fonte do código de alinhamento](https://css-tricks.com/quick-css-trick-how-to-center-an-object-exactly-in-the-center/) - Aqui foi onde encontrei o código para alinhamento com a propriedade `transform`. O engraçado é que isso foi postado a quase 15 anos atrás.

- [Explicação da propriedade __*transform*__](https://developer.mozilla.org/en-US/docs/Web/CSS/transform) - Isso vai te dar uma explicação sobre as funções da propriedade.

## Autor

Me siga para mais "soluções" :wink: 

- Frontend Mentor - [@braga-git](https://www.frontendmentor.io/profile/braga-git)
- Instagram - [@braga.jpeg](https://www.instagram.com/braga.jpeg/)
- LinkedIn - [Gabriel Braga Camara](https://www.linkedin.com/in/gabrielbragacamara/)

## Reconhecimentos

Gostaria de agradecer o [@chriscoyier](https://github.com/chriscoyier) pelo post sobre a propriedade `transform`. Eu tinha 6 anos na época! :joy:
