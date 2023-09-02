# Propriedades de Dimensionamento e Espaçamento

## Largura e Altura
Para estilizar largura e altura de um elemento nós utilizamos a propriedade width e height respectivamente.

Cada Propriedade tem seu **valor default**

Caso não saiba o valor default de determinada propriedade basta colocar **initial** no seu valor

```css
p {
    width: initial;
}
```

**Por padrão o valor default da propriedade width e height é auto**

## Largura e Altura minima e maxima
- max-width e min-width
- max-height e min - height

Usadas para poder limitar algum elemento
```css
button{
    background: pink;
    max-width: 200px;
    min-height: 50px;
    max-height: 100px;

}
```

## Valor inherit
Ao passar esse valor na propriedade height, ela utiliza a mesma altura do elemento pai. Esse valor se extende a outras propriedades CSS.
```css
button{
    width: inherit;
}
```


## Margin
É usada para criar um espaçamento pelas bordas de fora do nosso elemento

Para criar uma margem em cima, utilize margin-top
```
margin-top: valor;
```

Para criar uma margem na esquerda, utilize margin-left
```
margin-left: valor;
```
Para criar uma margem na direita, utilize margin-right
```
margin-right: valor;
```
Para criar uma margem embaixo, utilize margin-bottom
```
margin-bottom: valor;
```

### Propriedade Margin
Com a propriedade Margin eu consigo mexer na margem dos 4 cantos do elemento

**Aplicando 1 valor na propriedade Margin** ele automaticamente aplica esse valor de margem a todos os lados do elemento
```
margin: todosOsLados;
```

**Aplicando 2 valores na propriedade Margin** ele aplica em cima e em baixo o primeiro valor passado e nos lados o segundo valor
```
margin: CimaEBaixo Lados;
```

**Aplicando 3 valores na propriedade Margin** o primeiro valor ele aplica em cima, o segundo nas laterais e o terceiro embaixo
```
margin: Cima Lados Embaixo;
```
**Aplicando 4 valores na propriedade Margin** o primeiro em cima, o segundo na direita, o terceiro embaixo e o ultimo na esquerda
```
margin: Cima Direita Baixo Esquerda;
```

**OBS.:** Podemos trabalhar com valores negativos na Margin, fazendo o elemento sumir da pagina

## Parametro auto na propriedade Margin
Caso utilize essa propriedade ela centraliza o elemento na Horizontal
```
margin: auto;
```

Para centralizar na Horizontal e definir uma altura utilize mais um valor;
```
margin: CimaEBaixo auto;
```

# Padding
Ele cria um espaçamento entre o fundo e o Conteudo, os valores funcionam como a margin, ou seja, os valores são aplicados em sentido horario e também é possivel usar top, left, right e top, assim como valores negativos.

# Box Sizing
Utilizado para respeitar a largura e altura definidas, então quando alteramos o padding de um elemento, as vezes esse elemento "Aumenta" de tamanho, pois o calculo da largura é feito por
```
width = largura + borda + padding
```

Para que respeita a largura dada podemos usar o border-box
```
box-sizing: border-box;
```

Essa propriedade e valor, diminuem o valor da largura para poder dar o valor original





