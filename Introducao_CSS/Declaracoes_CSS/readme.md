# Propriedades e valores

- Propriedades: É uma caracteristica de um elemento no nosso HTML
- Valor: define o resultado de uma propriedade

Ex.: propriedade: valor;

```css
background: red;
color: white;
```

Os dois pontos ( : ) define o fim da declaração da Propriedade e o ponto e virgula ( ; ) define o fim da declaração do valor do estilo.

# Formas de Declarar o CSS

## Forma inline
Adicionamos o Código CSS utilizando o atributo Style dentro das tags HTML, elemento por elemento.

```html
<h1 style="background: red; color: white;"> Forma de Declaração inline</h1>
```

**OBS.:** Não é muito utilizavel pois não tem bom desempenho, porém se precisa testar uma propriedade rapidamente pode ser usado.

**OBS.2:** A declação Inline tem mais prioridade, ou seja, se tiver em outra declaração a que será usada é a que estiver Inline

## Forma CSS Interno
É adicionado dentro da Tag head da página HTML, onde colocamos a tag style

```html
    <style>
        h2{
            background: rgb(102, 255, 0);
            color: rgb(32, 32, 32);
        }
        
    </style>
</head>

<body>
    <h1 style="background: red; color: white;"> Forma de Declaração inline</h1>
    <h2> Forma de Declaração interna</h2>
    
</body>
</html>
```

**Desvantagem:** Dificulta a manutenção da nossa página e é dificil reutilizar os mesmos estilos

## Forma CSS externo
Maneira mais usada onde um arquivo com a extensão .css é criado e nele é armazenado os estilos.

Para utilizar essa forma precisamos linkar o css com o HTML, para isso usamos a tag link

```css
    <link rel="stylesheet" href=""> 
```   

O rel especifica qual a relação entre o documento atual e o outro

### Vantagem 
- Essa forma é mais usada pois a estrutura HTML fica melhor e com maior desempenho;
- Velocidade de carregamento mais rápida;
- Reaproveitamento de Estilo em outros projetos;
- Facilidade na Manutenção.

### Desvantagem
- Pelos arquivos serem renderizados separadamente, pode acontecer que em milessimos de segundos o seu HTML carregue primeiro que o CSS, mas isso vai depender da velocidade.

# Depurando o CSS
Esse processo é conhecido como Debug, é uma forma de identificar problemas no código-fonte de uma aplicação e entender seu comportamento, navegadores tem a ferramente **Dev Tools**, permitindo examinar os sistes, requisições, entre outros.

## Dev Tools
A aba Elements será usada para podermos depurar o CSS em conjunto com a Styles.

### Aba Styles
O que estiver em Italico é as propriedades de cada navegador.

### Aba Computed
Mostra todas as propriedades e seus valores, as que estiverem destacadas são as que estivermos colocado valores e estilizado, podemos também agrupar , ou desmarcar as duas Opções para poder ver apenas as que temos no elemento.

Podemos modificar as configurações direto pelo navegador, porém assim que editar é preciso colocar ela no arquivo css, se não ela será perdida ao recarregar a página

### Element Style
Coloca a propriedade apenas no elemento, caso queira para todos os elementos iguais a esse, é preciso achar a tag ou classe e alterar por ela, não pelo element.style

### Responsividade
Também conseguimos criar responsividade de acordo com os dispositivos selecionados
