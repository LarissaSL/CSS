# Agrupamento de Seletores
Os agrupamentos servem para podermos utilizar nosso codigo da melhor forma possivel, imagine que você deseja que o H1, Paragrafo e Div, tivessem a cor vermelha na fonte, você selecionaria um por vez e aplicaria a propriedade color:red.

```css
h1{
    color: red;
}

p{
    color: red;
}

div{
    color: red;
}
```

Para aproveitar o código é recomendado usar o agrupamento de seletores, assim apenas um unico bloco de codigo do css, será aplicado caso aja alterações. Conforme abaixo:
```css
h1, p, div{
    color: red;
}
```
**Note:** o código se reduziu e caso aja alterações fica muita mais fácil para realizar elas.

Podemos fazer esse agrupamentos, misturando os Tipos de Seletores.

```css
 p .texto{
    color: red;
}
```

Neste exemplo, eu estou selecionando todos os paragrafos que tenham a classe texto.

# Combinadores
Eles vão especificar qual o tipo de relacionamento entre os seletores

1. Combinador descendente (espaço)
2. Combinador filho (>)
3. Combinador irmão adjacente(+)
4. Combinador irmão em geral(~)

## Estrutura

```
[SELETOR] [COMBINADOR] [SELETOR]
```

### Combinador Descendente
```CSS
li li{
    color: green;
}
```
Neste exemplo, eu estou selecionando as tags Li que tenham outras tag Li

### Combinador Filho
Aplica apenas os estilos ao elemento que realmente é filho de outro
```CSS
div > p {
    color: green;
}
```


