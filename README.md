# Controladores Lógicos Programáveis e Redes Industriais

# Bom dia, Lorena.

## Hoje, 26 de setembro. Elabore o programa da seção exercícios

## Continue copiando o programa resolvido no CADERNO!!!

## Materiais

<a href=http://www.icos.com.br/downloads/manual-clp-clic-02-weg.pdf>Manual Clic02 - WEG </a>

<a href=https://github.com/mchavesferreira/cri/blob/main/Apostila%20CLP140IF%20vs2.5br.pdf>Manual da bancada CLP</a>

## Click02 - WEG

### Variáveis Digitais
<img src=img/variaveis_digitais.png>

### Variáveis Analógicas
<img src=img/variaveis_analogicas.png>

### Variáveis de Aplicação
<img src=img/instrucoes_aplicacao.png>


### Temporizador p. 14

### Contador p. 19

https://app.plcsimulator.online/




## EMENTA:

O componente curricular desenvolve conhecimentos relacionados aos sistemas industriaiscontrolados por CLP’s, com projetos utilizando linguagens apropriadas aos controladores lógicos
programáveis. Contempla conhecimentos sobre protocolos em redes industriais, interpretação de redes físicas e lógicas industriais

## OBJETIVOS:

Avaliar recursos e processos com CLP, bem como suas implicações; Correlacionar as propriedades e características das máquinas e equipamentos controlados por CLP, bem como as suas
aplicações. Conhecer e interpretar equipamentos. Identificar e trabalhar com redes de comunicação industrial.



## Controladores Lógicos Programáveis (CLP)

O Controlador Lógico Programável (CLP) foi criado na década de 1960, durante um período de grande avanço tecnológico na indústria. A primeira utilização significativa de CLPs foi na fábrica da General Motors em 1968, onde a necessidade de um sistema flexível para substituir os painéis de relés rígidos e complicados era evidente. O CLP proporcionou uma solução programável, que podia ser facilmente alterada conforme as necessidades de produção mudavam, sem a necessidade de extensa reconfiguração física.

<img src=https://raw.githubusercontent.com/mchavesferreira/scri/main/img/fabricarele.jpg><BR>Ilustração de uma fabrica com painéis rele/temporizador

Os CLPs rapidamente se tornaram populares devido às suas várias vantagens. Primeiramente, eles reduziram significativamente o tempo e o custo de reconfiguração de sistemas de controle, uma vez que modificações podiam ser feitas via software em vez de hardware. Além disso, os CLPs são altamente confiáveis e robustos, capazes de operar em ambientes industriais rigorosos com pouca manutenção.

Outra vantagem significativa é a capacidade de integração e expansão. CLPs podem ser facilmente conectados a outros sistemas e dispositivos, facilitando a implementação de soluções de automação complexas e escaláveis. A flexibilidade dos CLPs permite o uso de várias linguagens de programação padronizadas pela norma IEC 61131-3, tornando-os acessíveis a uma ampla gama de aplicações e profissionais.

<img src=https://raw.githubusercontent.com/mchavesferreira/cri/main/img/fabricaplc.jpg><BR>Ilustração de uma fabrica com PLC

Hoje, os CLPs continuam a ser um componente central na automação industrial, proporcionando controle eficiente e confiável para processos de manufatura, distribuição e muitos outros setores.

<img src=https://raw.githubusercontent.com/mchavesferreira/cri/main/img/fabrica40.jpg><BR>Ilustração de uma fabrica 4.0


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

Mobile Android:  https://play.google.com/store/apps/details?id=com.casdata.plcladdersimulator2&hl=pt


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


# Exercícios

# 26/09/2024

1)	Uma empresa contratou você para fazer a programação de um novo equipamento adquirido. A máquina é uma selecionadora de peças (metálica e não metálica) e sua programação funciona da seguinte forma:

•	Ao pressionar o botão de START a esteira M liga, assim deslocando a peça através da esteira;
•	Os sensores S1 e S2 são utilizados para identificar o tipo de material, metálico ou não metálico.
o	S1: sensor indutivo – detecção de material metálico
o	S2: sensor capacitivo – detecção de material metálico e não metálico
•	C1 e C2 são cilindros de simples ação;
•	O compartimento 1 é utilizado para armazenar material metálico;
•	O compartimento 2 é utilizado para armazenar material não metálico;
•	Os sensores S3 e S4 são sensores ópticos utilizados para identificar o material que foi armazenado;
•	O botão STOP para o processo, desligando a esteira e cilindros. 

<img src=img/esteira.png>

Desenvolva um programa em Ladder capaz de realizar tal tarefa.

| Variável de entrada        | Endereço CLP |   | Variável de saída | Endereço CLP |
|----------------------------|--------------|---|-------------------|--------------|
| Botão START (push-button)   | I01          |   | Esteira M         | Q01          |
| Botão STOP (push-button)    | I02          |   | C1                | Q02          |
| S1                         | I03          |   | C2                | Q03          |
| S2                         | I04          |   |                   |              |
| S3                         | I05          |   |                   |              |
| S4                         | I06          |   |                   |              |


## 19/09/2024

Em uma determinada indústria necessita de um sistema de separação de peças por tamanho.  Desenvolva o programa em linguagem Ladder” para um CLP, com as seguintes condições: 

a) ao pressionar o botão "start", uma peça cai no meio da esteira e, após 2 segundos para estabilizar, os sensores S3 e S4 verificam a altura da peça; 

b) se a peça for baixa (S3 acionado), aciona a esteira para um lado (Q2). Se a peça for alta (S3 e S4 acionados), aciona a esteira para outro lado (Q1); 

c) quando a peça passar pelo sensor da caixa apropriada, finaliza o ciclo e a esteira para (dá condição para um novo ciclo); 

d) a lâmpada liga enquanto o ciclo estiver em funcionamento. O botão "stop" finaliza o ciclo a qualquer instante. 
 
<img src=img/clptamanho.png>

## 12/09/2024

Exercício: <a href=https://github.com/mchavesferreira/cri/blob/main/atividade_ladder.pdf>exemplo de projeto</a> com CLP, porém crie uma tela onde apareça o nome da empresa, e os valores de tempo  e peças de forma que possam ser alterados.

<img src=https://raw.githubusercontent.com/mchavesferreira/cri/main/img/ihmmoteleone.png>

Após esta implementação, inclua telas que informem em texto as condições de ligado e desligado Valvulas e ventilador, separando em telas de H02, H03...


## Links de auxilio

Microcontroladores Atmega e placa ESP32

<img src=https://github.com/mchavesferreira/img/blob/main/logogpt.png> https://chatgpt.com/g/g-TFvuISQH5-professor-dos-embarcados

<img src=https://github.com/mchavesferreira/img/blob/main/logogpt.png>  https://chatgpt.com/g/g-thK1Ja9RM-referencias-de-artigos-normas-abnt-nbr

Norma IEC-61131-3: https://plcopen.org/sites/default/files/downloads/intro_iec_march04_portuguese.pdf



