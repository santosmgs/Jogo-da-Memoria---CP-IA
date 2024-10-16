## Jogo Genius com Arduino

Para esse checkpoint de IA implementamos um jogo de memória semlhante ao jogo "Genius" usando o Arduino.

### Funcionalidades

- Sequências de luzes e sons que o jogador precisa repetir.
- Níveis de dificuldade crescente.
- Feedback visual e sonoro para acertos e erros.
- Reinício automático após o término do jogo.

### Requisitos

- Arduino Uno
- 4 LEDs
- 4 Resistores de 220 ohms (o padrão que geralmente é usado)
- 4 Botões
- 1 Buzzer
- Protoboard
- Fios Jumper

### Esquema de Conexões

**LEDs:**

- LED 1: Pino 8
- LED 2: Pino 9
- LED 3: Pino 10
- LED 4: Pino 11

**Botões:**

- Botão 1: Pino 2
- Botão 2: Pino 3
- Botão 3: Pino 4
- Botão 4: Pino 5

**Buzzer:**

- Pino 12

**Observação:** Conecte os LEDs e o buzzer através dos resistores de 220 ohms.

### Instalação

1. Faça o download ou clone este repositório.
2. Abra o arquivo `genius.ino` no Arduino IDE.
3. Conecte seu Arduino ao computador.
4. Selecione a placa e a porta serial corretas no Arduino IDE.
5. Faça o upload do código para o Arduino.

### Como Jogar

1. Pressione qualquer botão para iniciar o jogo.
2. O Arduino irá gerar uma sequência aleatória de luzes e sons.
3. Repita a sequência pressionando os botões correspondentes.
4. Se você acertar a sequência, o jogo avança para o próximo nível com uma sequência mais longa.
5. Se você errar a sequência, o jogo termina e você precisa reiniciá-lo.

### Funcionamento e features

O código está dividido em diversas funções e algumas features:

- `reiniciar()`: Reinicia o jogo para o estado inicial.
- `escolhaErrada()`: Executada quando o jogador erra a sequência.
- `mostrarSequencia()`: Exibe a sequência atual de luzes e sons.
- `verificar()`: Verifica se a escolha do jogador está correta.
- `setup()`: Inicializa as configurações do Arduino.
- `loop()`: Loop principal do programa.

### Observações

- O código utiliza `delay()` para controlar o tempo, o que pode causar atrasos no loop principal.

### Site utilizado para simulação

- Tinkercard


