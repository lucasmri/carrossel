# Carrossel

Este é um carrossel simples desenvolvido utilizando HTML, CSS e JavaScript, projetado para uso em desktops e laptops.

## Demonstração Visual

![Demonstração](https://github.com/user-attachments/assets/a77d4b51-b58b-4010-a361-39c34162afcb)

## Stack utilizada

**Front-end:** HTML5, CSS3, JavaScript

## Funcionalidades

- Imagens personalizadas
- Tempo de duração das imagens editáveis

## Instalação / Download

Para baixar o projeto, execute o seguinte comando git clone no diretório onde deseja salvar o projeto:

```bash
  git clone https://github.com/lucasmri/carrossel.git
```

## Como utilizar?

Após o download, abra o arquivo `index.html` em um navegador para usar o carrossel. As imagens serão trocadas automaticamente ou você pode acelerar o processo clicando nos botões laterais do modal. Use o botão `L` para retroceder uma imagem e o botão `R` para avançar.


## Como alterar as imagens?

Para alterar as imagens, edite o arquivo `.css` e modifique a `URL` na classe correspondente à ordem de cada imagem desejada. Por exemplo, a classe `slide1` refere-se à primeira imagem do carrossel, a classe `slide2` à segunda, e assim por diante.

```css
  .slide1 {
    background: url("link-aqui") no-repeat center center;
    background-size: cover;
}
``` 

## Como editar o tempo de duração de cada imagem?

Para alterar a duração de exibição das imagens é necessário alterar o arquivo `.js` e localizar a função correspondente à imagem que deseja modificar. Por exemplo, a função `slide1()` refere-se à primeira imagem, a função `slide2()` à segunda, e assim por diante. Depois de encontrar a função, altere o segundo parâmetro do `setTimeout` para o tempo desejado em milissegundos. Por exemplo, se colocar 7000 será equivalente a 7 segundos.

```javascript
  function slide1() {
    slide.setAttribute("class","slide1");
    timer = setTimeout(slide2,tempo-aqui);
    nCheck = 1;
}
``` 