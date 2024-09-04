# Identificador de Melhor Cor de Texto para Fundo Colorido

Este projeto permite aos usuários selecionar uma cor de fundo e uma cor de texto base, ajustando automaticamente a cor do texto para garantir o melhor contraste com o fundo escolhido. O ajuste da cor do texto é feito de forma a garantir uma boa legibilidade.

## Funcionalidades

- Seleção de cor de fundo através de um seletor de cores.
- Seleção de cor base do texto através de um seletor de cores.
- Ajuste automático da cor do texto para maximizar o contraste e garantir legibilidade.
- Exibição da cor do texto escolhida no formato hexadecimal.

## Tecnologias Utilizadas

- **HTML5**: Estrutura básica da página.
- **CSS3**: Estilização do layout e dos elementos.
- **JavaScript**: Lógica para ajuste automático da cor do texto baseado na cor de fundo e na cor base do texto.

## Como Funciona

1. O usuário seleciona uma cor de fundo usando o seletor de cor.
2. O usuário seleciona uma cor base para o texto usando outro seletor de cor.
3. A aplicação calcula o contraste entre a cor de fundo e a cor base do texto. Se o contraste for baixo, a cor do texto é ajustada automaticamente para um valor mais adequado:
   - Se o fundo for claro, a cor do texto será escurecida.
   - Se o fundo for escuro, a cor do texto será clareada.
4. A cor final do texto é exibida na área de saída com a frase de exemplo: "Lorem ipsum dolor sit."

## Funções Principais

### `calculateLuminance(r, g, b)`
Calcula a luminância relativa de uma cor baseada em seus valores RGB. A luminância é usada para calcular o contraste.

### `getRGB(hex)`
Converte uma cor em formato hexadecimal para o formato RGB.

### `rgbToHex(r, g, b)`
Converte uma cor RGB para o formato hexadecimal.

### `adjustBrightness([r, g, b], factor)`
Ajusta o brilho de uma cor RGB com base em um fator fornecido (0 para escurecer, 255 para clarear).

### `getContrastRatio(l1, l2)`
Calcula a razão de contraste entre duas luminâncias.

### `chooseTextColor(backgroundColor, baseTextColor)`
Seleciona a cor do texto com base no contraste entre a cor de fundo e a cor base do texto. Ajusta a cor do texto automaticamente se o contraste for insuficiente.

## Como Usar

1. Clone este repositório ou copie o código HTML para seu ambiente de desenvolvimento.
2. Abra o arquivo `index.html` em um navegador.
3. Utilize os seletores de cor para escolher uma cor de fundo e uma cor base de texto.
4. A cor do texto será ajustada automaticamente para garantir um bom contraste com a cor de fundo.

## Exemplo de Uso

Selecione uma cor de fundo e uma cor base para o texto:

- Se o fundo for claro, a cor do texto será escurecida para melhorar a legibilidade.
- Se o fundo for escuro, a cor do texto será clareada.

## Requisitos

- Um navegador moderno com suporte a HTML5, CSS3 e JavaScript.

## Licença

Este projeto está licenciado sob a licença MIT. Sinta-se à vontade para usá-lo e modificá-lo conforme necessário.
