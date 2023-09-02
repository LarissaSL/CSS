# Seletores CSS
No CSS os seletores tem como objetivo definir quais elementos nós vamos selecionar para aplicar o Estilo

- **Seletor de Tag/Tipo:** Busca por uma tag HTML especifica
```css
div {
    propriedade: valor;
}
```
- **Seletor de ID:** Deve ser unico dentro da Página HTML, é usado a hashetag ( # ) para selecionar
```css
#nome-do-id {
    propriedade: valor;
}
```
Neste exemplo, as tags que tiverem o nome desse ID terão os valores da propriedade.

- **Seletor de Classes:** Podemos repetir as classes em varias tags, é utilizado o ponto ( . ) para selecionar.
```css
.nome-da-classe{
    background: red;
    color: white;
}
```
Neste exemplo, as tags que tiverem o nome dessa classe terão um fundo vermelho e cor branca na fonte.

**É possivel utilizar mais de uma classe na tag.**

Exemplo:
```html
<p class="seletor-por-classe texto-maiusculo"></p>
<p class="seletor-por-classe"></p>
```

```css
.seletor-por-classe{
    background: red;
    color: white;
}

.texto-maiusculo{
    text-transform: uppercase;
}
```

Neste exemplo, os dois paragrafos terão um fundo vermelho e cor branca na fonte, porém o primeiro estará com o texto maiusculo.
- **Seletor Universal:** Ele seleciona todos os elementos de um documento HTML, independente de ter classe, id, etc.
Esse seletor é asterisco ( * )
```css
*{
    font-weight: bold;
}
```
Neste exemplo todos os textos estarão em Negrito
- **Seletor de Atributo:** Podemos utilizar o seletor por atributo, é usado o colchetes ( [] )para selecionar
Exemplo:
```html
<a title="Streaming Prime" href="https://www.primevideo.com/"></a>
```

```css
[title]{
    color: white;
}

[title="Streaming Prime"]{
    color: blue;
}

[title~="Streaming"]{
    color: blue;
}
```
Neste exemplo, todos os elementos Title terão cor Branca e todos os elementos title que forem prime, terão a cor Azul. No terceiro Seletor, ele procura a palavra exata ou o valor que tenha a palavra separada por espaço.
