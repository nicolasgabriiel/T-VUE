## TAMANHOS, WIDTH E HEIGHT

**Pixels (px):** Uma unidade de medida fixa que representa um único pixel na tela.

**Porcentagem (%):** Define um tamanho ou altura em relação a um elemento pai. Por exemplo, width: 50% significa metade da largura do elemento pai.

**Em (em):** Relaciona o tamanho ao tamanho da fonte do elemento pai. Um valor de 1em é igual ao tamanho da fonte atual do elemento pai.

**Rem (rem):** Semelhante ao "em", mas relaciona o tamanho à raiz (root) do documento HTML, tornando-o mais previsível e fácil de controlar.

**Viewport Width (vw):** Define o tamanho em relação à largura da janela de visualização do navegador. Por exemplo, width: 10vw representa 10% da largura da janela de visualização.

**Viewport Height (vh):** Semelhante ao "vw", mas relaciona o tamanho à altura da janela de visualização.

**Viewport Min (vmin):** Define o tamanho com base na largura ou altura da janela de visualização, dependendo de qual dimensão é menor.

**Viewport Max (vmax):** Define o tamanho com base na largura ou altura da janela de visualização, dependendo de qual dimensão é maior.

**Centímetros (cm):** Uma unidade de medida baseada em centímetros físicos.

**Milímetros (mm):** Uma unidade de medida baseada em milímetros físicos.

**Polegadas (in):** Uma unidade de medida baseada em polegadas físicas.

**Pontos (pt):** Uma unidade de medida usada principalmente para tamanho de fonte, onde 1 ponto é aproximadamente igual a 1/72 de polegada.

**Picas (pc):** Uma unidade de medida usada principalmente para tamanho de fonte, onde 1 pica é igual a 12 pontos.

**Unidades de tela (vw, vh, vmin, vmax):** Estas unidades são relacionadas ao tamanho da tela do dispositivo e são usadas para criar layouts responsivos.

**Porcentagem de altura da viewport (vh):** Permite definir alturas em relação à altura da janela de visualização. 



## POSITION

**position: static:**
-É o valor padrão para todos os elementos em uma página.
-O elemento é posicionado de acordo com o fluxo normal do documento.
-As propriedades top, right, bottom e left não têm efeito em elementos com position: static.
-Não é afetado por outros elementos posicionados.

**position: relative:**
-O elemento é posicionado em relação à sua posição normal no fluxo do documento.
-Pode ser deslocado usando as propriedades top, right, bottom e left, que definem a distância em relação à sua posição normal.
-Mesmo que você desloque o elemento, ele ainda ocupa espaço em seu local original no layout.

**position: absolute:**
-O elemento é posicionado em relação ao elemento pai mais próximo com uma posição diferente de static.
-Pode ser deslocado usando as propriedades top, right, bottom e left, que definem a distância em relação ao elemento pai posicionado.
-O elemento não ocupa espaço em seu local original no layout, e outros elementos podem ocupar seu espaço.
-Se nenhum ancestral com uma posição diferente de static for encontrado, o elemento será posicionado em relação ao elemento raiz do documento (geralmente a tag <html></html>).


## DISPLAYS

**display: block:**
-Elementos com display: block são chamados de "elementos de bloco".
-Eles são renderizados em uma nova linha e ocupam a largura total do contêiner pai.
-Eles geralmente começam em uma nova linha, empurrando elementos anteriores e seguintes para suas próprias linhas.
-Exemplos comuns de elementos de bloco incluem <div>, <p>, <h1>, <ul>, <li> e muitos outros elementos de conteúdo.

**display: inline:**
-Elementos com display: inline são chamados de "elementos inline".
-Eles são renderizados na mesma linha e ocupam apenas o espaço necessário para o conteúdo.
-Elementos inline não podem receber largura ou altura, e não podem iniciar uma nova linha.
-Exemplos de elementos inline incluem <span>, <a>, <strong>, <em>, <img>, entre outros.

**display: inline-block:**
-Elementos com display: inline-block combinam características de elementos de bloco e elementos inline.
-Eles são renderizados na mesma linha, mas podem receber largura e altura, permitindo o controle do layout.
-Elementos inline-block não iniciam uma nova linha e podem coexistir lado a lado, semelhante aos elementos inline.
-É útil quando você deseja elementos com um layout personalizado dentro do fluxo de texto, como botões ou elementos de caixa.


## Posicionar Imagens com relação ao Texto

## 1 - float:

A propriedade float é usada para criar layouts onde os elementos podem "flutuar" ao redor de outros elementos. Pode ser aplicada a elementos de bloco, como imagens. Aqui estão alguns conceitos-chave:

**float: left;:** Isso faz com que o elemento flutue para a esquerda, permitindo que o texto flua à direita da imagem.

**float: right;:** Isso faz com que o elemento flutue para a direita, permitindo que o texto flua à esquerda da imagem.

Elementos flutuantes não ocupam espaço vertical em seus contêineres pai, portanto, você pode precisar limpar as flutuações usando a propriedade clear em elementos subsequentes.


## 2 - display: inline e display: block:
A propriedade display controla como um elemento é renderizado no layout. É comum usar display: inline para imagens embutidas em texto e display: block para imagens que devem começar em uma nova linha.

**display: inline;:** Isso faz com que o elemento seja renderizado na mesma linha que o texto e ocupe apenas o espaço necessário.

**display: block;:** Isso faz com que o elemento seja renderizado em uma nova linha e ocupe a largura total do contêiner.


## 3 - position: relative e position: absolute:
As propriedades position: relative e position: absolute podem ser usadas para posicionar imagens em relação ao texto ou a outros elementos. Aqui estão os conceitos-chave:

**position: relative;:** Isso permite ajustar a posição de um elemento em relação à sua posição normal. Você pode usar as propriedades top, right, bottom e left para definir o deslocamento em relação à posição normal.
**position: absolute;:** Isso posiciona o elemento em relação ao elemento pai mais próximo com uma posição não static. Você pode usar as propriedades top, right, bottom e left para definir o posicionamento preciso.


## 4 - Usar Imagens como Plano de Fundo:
Você pode usar imagens como plano de fundo para elementos de texto, como parágrafos, usando a propriedade **background-image**. Isso permite que o texto fique sobre a imagem de plano de fundo. Você pode controlar a posição da imagem de plano de fundo com as propriedades background-position, background-repeat e outras relacionadas à imagem de plano de fundo.


## ALINHAMENTOS

**text-align:**
A propriedade text-align é usada para controlar o alinhamento horizontal do texto dentro de um elemento. Pode ser aplicada a elementos de bloco ou em linha.
Valores possíveis são:
   **-left:** Alinha o texto à esquerda.
   **-right:** Alinha o texto à direita.
   **-center:** Alinha o texto ao centro.
   **-justify:** Justifica o texto, criando margens retas em ambos os lados do texto.

**text-align-last:**
A propriedade text-align-last é usada para controlar o alinhamento do último fragmento de texto em um elemento.
Valores possíveis são semelhantes aos de text-align: left, right, center, justify

**vertical-align:**
A propriedade vertical-align é usada para controlar o alinhamento vertical de elementos de texto em relação ao texto vizinho ou ao contêiner. Ela é frequentemente usada com elementos inline e elementos de imagem.
Valores possíveis incluem baseline, top, middle, bottom, text-top, text-bottom e valores numéricos.

**line-height:**
A propriedade line-height controla a altura da linha de texto. Você pode ajustar essa propriedade para controlar o espaçamento vertical entre as linhas de texto, afetando indiretamente o alinhamento vertical do texto.


## Estilos de Fontes

**font-family:**
A propriedade font-family define a família de fontes a ser usada para o texto em um elemento. Você pode listar várias fontes de fallback em caso de a fonte preferida não estar disponível no sistema do usuário.

**font-size:**
A propriedade font-size determina o tamanho da fonte do texto em um elemento. Você pode definir o tamanho em pixels, em, porcentagem ou outras unidades.

**font-weight:**
A propriedade font-weight define a espessura da fonte, permitindo que você escolha entre pesos como "normal", "bold", "bolder" ou valores numéricos.

**font-style:**
A propriedade font-style controla o estilo da fonte, permitindo que você escolha entre "normal", "italic" e "oblique".

**text-transform:**
A propriedade text-transform define como o texto é transformado em maiúsculas ou minúsculas. Valores incluem "uppercase", "lowercase" e "capitalize".

**text-decoration:**
A propriedade text-decoration controla a decoração do texto, como sublinhado, linha através do texto e outros efeitos. Valores incluem "underline", "overline" e "line-through".

**line-height:**
A propriedade line-height define a altura da linha, controlando o espaçamento entre as linhas de texto.

**letter-spacing:**
A propriedade letter-spacing ajusta o espaçamento entre as letras do texto.

**word-spacing:**
A propriedade word-spacing ajusta o espaçamento entre as palavras do texto.

**text-align:**
A propriedade text-align controla o alinhamento horizontal do texto em um elemento. Pode ser "left", "right", "center" ou "justify".


## DIFERENÇA ENTRE UNIDADES DE MEDIDAS

## - Unidades Absolutas:

**Pixels (px): Uma unidade de medida fixa que representa um único pixel na tela. É uma unidade absoluta porque tem um valor fixo e não muda em relação ao tamanho da janela ou dispositivo. Vantagem: precisão total no controle de tamanhos.

## - Unidades Relativas:

**Porcentagem (%):** Define o tamanho em relação a um valor de referência, como o elemento pai. Por exemplo, width: 50% significa metade do tamanho do elemento pai. Vantagem: layouts responsivos e flexíveis, adaptando-se ao tamanho do contêiner pai.
**Em (em):** Relaciona o tamanho ao tamanho da fonte do elemento pai. Um valor de 1em é igual ao tamanho da fonte atual do elemento pai. Vantagem: escalabilidade com base na fonte, permitindo layouts de texto proporcionais.
**Rem (rem):** Semelhante ao "em", mas relaciona o tamanho à raiz (root) do documento HTML, tornando-o mais previsível e fácil de controlar. Vantagem: consistência em todo o documento.
**Viewport Width (vw):** Define o tamanho em relação à largura da janela de visualização do navegador. Por exemplo, width: 10vw representa 10% da largura da janela de visualização. Vantagem: layout responsivo em relação ao tamanho da tela.
**Viewport Height (vh):** Semelhante ao "vw", mas relaciona o tamanho à altura da janela de visualização. Vantagem: layout responsivo em relação à altura da tela.
**Viewport Min (vmin):** Define o tamanho com base na largura ou altura da janela de visualização, dependendo de qual dimensão é menor. Vantagem: adaptação a ambas as dimensões da tela.
**Viewport Max (vmax):** Define o tamanho com base na largura ou altura da janela de visualização, dependendo de qual dimensão é maior. Vantagem: adaptação a ambas as dimensões da tela.

## - Unidades de Texto:

**Polegadas (in), Centímetros (cm), Milímetros (mm), Pontos (pt) e Picas (pc):** Essas unidades são baseadas em medidas físicas e são usadas principalmente para controle preciso de tamanhos de fonte e layout de impressão. Vantagem: úteis para design impresso e absoluto controle de tamanho.

## - Outras Unidades Específicas:

**Pixel Relativo (rem):** Relaciona o tamanho da fonte à raiz (root) do documento, fornecendo uma unidade de medida relativa em relação à fonte raiz do documento. Isso é particularmente útil para criar layouts escaláveis e consistentes em toda a página.
A escolha da unidade de medida depende dos requisitos do layout e do comportamento responsivo desejado. Unidades relativas, como porcentagem, em e rem, são frequentemente preferidas para layouts flexíveis e responsivos, enquanto unidades absolutas, como pixels, podem ser usadas para tamanhos fixos e precisos. As unidades de texto e de visualização (vw, vh, vmin, vmax) são especialmente úteis em contextos de design responsivo, adaptando-se às dimensões da tela do dispositivo.


## SELETORES CSS


**1 Seletores de ID:**
Os seletores de ID são indicados pelo caractere "#" seguido do nome do ID (por exemplo, #meu-id).
Têm a maior prioridade e sobrescreverão qualquer estilo definido por seletores de classe ou elementos.

**2 Seletores de Classe:**
Os seletores de classe são indicados por um ponto (por exemplo, .minha-classe).
Têm uma prioridade menor do que os seletores de ID, mas uma prioridade maior do que os seletores de elementos.

**3 Seletores de Elemento:**
Os seletores de elemento visam um tipo específico de elemento HTML (por exemplo, p, h1, div).
Têm uma prioridade menor do que seletores de classe e ID.

**4 Seletores de Descendência:**
Os seletores de descendência permitem estilizar elementos com base em sua hierarquia no documento HTML. Por exemplo, p a selecionará todos os elementos âncora (<a>) que estão dentro de um parágrafo (<p>).
Têm uma prioridade menor do que os seletores de elemento simples.

**5 Seletores de Filho Direto:**
Os seletores de filho direto selecionam elementos que são filhos diretos de outro elemento. Por exemplo, div > p selecionará todos os parágrafos (<p>) que são filhos diretos de uma divisão (<div>).
Têm uma prioridade maior do que os seletores de descendência.

**6 Seletores de Classe Pseudo-elemento:**
Os seletores de classe pseudo-elemento são usados para estilizar partes específicas de elementos. Por exemplo, p::first-line selecionará a primeira linha de todos os parágrafos (<p>).
Têm uma prioridade menor do que os seletores de classe, ID e elemento, mas uma prioridade maior do que os seletores de classe pseudo-classe.

**7 Seletores de Classe Pseudo-classe:**
Os seletores de classe pseudo-classe são usados para selecionar elementos com base em estados ou interações específicas, como :hover para estilizar elementos quando o mouse passa por cima.
Têm uma prioridade menor do que os seletores de classe, ID, elemento e classe pseudo-elemento.



# TIPOS DE HOVER

**hover em Links:** O :hover é frequentemente usado em links para criar efeitos visuais quando o mouse passa sobre eles.

**:hover em Botões:** Você pode aplicar efeitos semelhantes a botões, como alterar cores de fundo, bordas e sombras quando o mouse passa sobre eles.

**:hover em Caixas de Texto:** Pode ser aplicado a caixas de texto, como campos de formulário ou áreas de texto, para criar efeitos de destaque quando o mouse passa sobre eles.

**:hover em Imagens:** Quando o mouse passa sobre uma imagem, você pode criar efeitos como zoom, transições suaves ou até mesmo substituir a imagem por outra.




# BOX SIZING

**content-box (valor padrão):**
Nesse modo, as dimensões de um elemento são calculadas a partir da borda externa do elemento. Ou seja, as dimensões não incluem a largura da borda e o preenchimento do elemento. Isso significa que, se você definir uma largura de 100 pixels, a largura total do elemento será 100 pixels mais a largura da borda e o preenchimento.

**border-box:**
Nesse modo, as dimensões de um elemento são calculadas a partir da borda interna do elemento. Isso significa que as dimensões incluem a largura da borda e o preenchimento. Se você definir uma largura de 100 pixels, a largura total do elemento será 100 pixels, e o conteúdo será dimensionado para caber dentro, descontando a largura da borda e o preenchimento.

A escolha entre content-box e border-box depende das necessidades do seu layout. border-box é frequentemente preferido para layouts responsivos, pois facilita a previsão das dimensões reais dos elementos, enquanto content-box é mais comum em layouts tradicionais onde você deseja controlar a largura do conteúdo independentemente da borda e do preenchimento.



## FLEXBOX

**Contêiner (Elemento Pai):**
O elemento que envolve os itens flexíveis é chamado de contêiner flex.
Você aPlica display: flex ou display: inline-flex ao contêiner para ativar o layout flexível.

**Itens Flexíveis (Elementos Filhos):**
Os elementos dentro do contêiner flex são chamados de itens flexíveis.
Os itens flexíveis são organizados em relação uns aos outros, ajustando-se ao tamanho do contêiner e distribuindo espaço de acordo com as regras definidas.

**Eixo Principal e Transversal:**
O Flexbox opera em dois eixos: o eixo principal e o eixo transversal.
O eixo principal é definido com base na direção do contêiner flex. Por padrão, é horizontal (da esquerda para a direita).
O eixo transversal é perpendicular ao eixo principal (vertical, de cima para baixo).

**Propriedades Importantes:**
Algumas propriedades-chave do Flexbox incluem justify-content (alinhamento no eixo principal), align-items (alinhamento no eixo transversal), flex-direction (direção do layout), flex-wrap (quebra de linha) e flex (para definir a flexibilidade dos itens).

**Alinhamento e Distribuição:**
O Flexbox fornece um controle preciso sobre o alinhamento e a distribuição de elementos, tornando-o ideal para a criação de layouts complexos, como menus, barras laterais, cabeçalhos e rodapés flexíveis.

**Layout Responsivo:**
O Flexbox é uma ferramenta poderosa para criar layouts responsivos, permitindo que os elementos se ajustem automaticamente ao tamanho da tela e ao conteúdo.



## GRID

**Contêiner Grid:**
Para criar um layout com Grid, você define um elemento HTML como o contêiner Grid aplicando a propriedade display: grid; a ele. Este contêiner se torna o contexto para o layout Grid.

**Linhas e Colunas:**
No Grid, você define linhas e colunas para dividir o espaço do layout. Você pode especificar o número, tamanho e posição das linhas e colunas. Pode haver linhas explícitas (definidas pelo desenvolvedor) e linhas implícitas (geradas automaticamente).

**Itens Grid:**
Os elementos filhos dentro do contêiner Grid são chamados de itens Grid. Você controla a posição e o tamanho desses itens no layout Grid, especificando em qual linha e coluna eles devem ser colocados.

**Posicionamento de Itens:**
Você pode posicionar itens Grid usando propriedades como grid-row e grid-column, que especificam em qual linha e coluna um item deve ser colocado. Além disso, você pode usar atalhos como grid-area para definir ambas as propriedades em uma única declaração.

**Alinhamento de Itens:**
O Grid oferece recursos de alinhamento que permitem controlar como os itens são alinhados nas células do Grid. Isso inclui alinhamento no eixo horizontal e vertical.

**Responsividade:**
O Grid é altamente responsivo, permitindo que os layouts se ajustem a diferentes tamanhos de tela. Você pode criar layouts que mudam automaticamente com base no espaço disponível.

**Aninhamento:**
Você pode aninhar Grids dentro de outros Grids, criando layouts complexos e aninhados.

**Grid Template Areas:**
O Grid oferece uma maneira intuitiva de definir layouts usando áreas nomeadas. Isso facilita a criação de layouts complexos com nomes de áreas legíveis e facilmente mantidos.