# Controladores Lógicos Programáveis e Redes Industriais

### Código: CRI

## EMENTA:

O componente curricular desenvolve conhecimentos relacionados aos sistemas industriaiscontrolados por CLP’s, com projetos utilizando linguagens apropriadas aos controladores lógicos
programáveis. Contempla conhecimentos sobre protocolos em redes industriais, interpretação de redes físicas e lógicas industriais

## OBJETIVOS:

Avaliar recursos e processos com CLP, bem como suas implicações; Correlacionar as propriedades e características das máquinas e equipamentos controlados por CLP, bem como as suas
aplicações. Conhecer e interpretar equipamentos. Identificar e trabalhar com redes de comunicação industrial.

# Lorena, hoje 08 de Agosto,
## vamos revisar alguns conceitos, apresentando alguns slides já disponibilizados e considerando os conceitos a seguir!

## Controladores Lógicos Programáveis (CLP)

## Linguagem de programação para os CLP

A IEC 61131-3 é um padrão internacional que estabelece diretrizes para as linguagens de programação usadas em controladores.

Este padrão especifica cinco linguagens de programação que podem ser aplicadas a qualquer Controlador Lógico Programável (CLP), independentemente de seu fabricante.

A IEC 61131 é uma norma detalhada e organizada em várias seções, cada uma tratando de diferentes aspectos dos controladores programáveis.

As linguagens consistem de 2 textuais:

- Instruction List (IL) / Lista de Instruções
- Structured Text (ST) / Texto Estruturado

3 gráficas:

- Ladder Diagram (LD)  / Diagrama Ladder
- Function Block Diagram (FBD) / Diagrama de Blocos Funcionais
- Sequential Function Chart (SFC) / Sequenciamento Gráfico de Funções


  
![linguagensplc](https://github.com/user-attachments/assets/235dc890-2fb2-4f0f-932c-c609b343c521)

![sfc](https://github.com/user-attachments/assets/266578d0-4179-4e64-8fae-10e7609e5bec)
  

# Linguagem LADDER

Vamos iniciar com a linguagem Ladder e utilizar simuladores online para a prática com esta linguagem:

PLC Simulator Online  https://app.plcsimulator.online/

## Ramificações e Links em Diagramas Ladder

Diagramas Ladder são uma parte essencial da programação de controladores lógicos programáveis (CLP) e são amplamente utilizados para representar a lógica de circuitos de controle elétrico. Dentro desses diagramas, ramificações e links desempenham um papel crucial na definição do fluxo de controle.

## Elementos de Link: Conceitos Básicos

Conforme definido na IEC-61131-3, os elementos de link podem ser horizontais ou verticais, com estados denotados como LIGADO ou DESLIGADO. Os elementos de link são integrais na transmissão de estados e são sinônimos de fluxo de energia, que é representado pela cor verde durante a simulação.

![rung-with-comments](https://github.com/user-attachments/assets/b53f84f9-0d37-4cc2-8e76-e86712ec65fd)


### Elementos de Link Horizontais:
- Representados por uma linha horizontal.
- Transmitem o estado da esquerda para a direita.

### Elementos de Link Verticais:
- Consistem em linhas verticais que intersectam links horizontais.
- Representam o OR inclusivo dos estados LIGADOS dos links horizontais à esquerda.
- Links verticais são usados para criar ramificações.

## Ramificação em Diagramas Ladder

A ramificação permite caminhos paralelos dentro do diagrama ladder. Utilizando elementos de link verticais, pode-se criar ramificações que permitem que múltiplas condições sejam verificadas simultaneamente.

### Criando Ramificações:
- Arraste e solte a ramificação da barra de ferramentas sobre o degrau ou elemento.
- Adicione novos elementos à ramificação inferior.
- O estado do link vertical representa o OR inclusivo dos estados LIGADOS dos links horizontais à sua esquerda.
- O estado do link vertical é copiado para todos os links horizontais conectados à sua direita. O estado LIGADO é representado pela cor verde durante a simulação.

## Aplicações Práticas

Ramificações e links permitem que a lógica de controle complexa seja representada visualmente em um diagrama ladder. Eles permitem verificações e operações simultâneas, proporcionando flexibilidade no design de sistemas de controle.

### Exemplos:
- Conexão em série de contatos (E)
- Conexão em paralelo de contatos (OU)
- Ramificações aninhadas
- Controle de partida/parada de motor com sustentação

## Conclusão

No campo da programação de CLPs, ramificações e links em diagramas ladder são fundamentais. Elementos de link horizontais transmitem estados e links verticais permitem a ramificação, permitindo que a lógica complexa seja organizada e visualizada. Essa abordagem proporciona a capacidade de gerenciar múltiplas condições de uma vez, oferecendo flexibilidade e eficiência no design de sistemas de controle. Seja em ramificações paralelas ou condições aninhadas, o uso de ramificações e links simplifica a compreensão de circuitos complexos. A combinação desses elementos resulta em uma representação coerente e acessível, tornando a tarefa de projetar e solucionar problemas em controles elétricos mais intuitiva e eficaz.


## Links de auxilio

IA para códigos microcontroladores Atmega e placa ESP32
https://chatgpt.com/g/g-TFvuISQH5-professor-dos-embarcados

https://chatgpt.com/g/g-thK1Ja9RM-referencias-de-artigos-normas-abnt-nbr

Norma IEC-61131-3: https://plcopen.org/sites/default/files/downloads/intro_iec_march04_portuguese.pdf



