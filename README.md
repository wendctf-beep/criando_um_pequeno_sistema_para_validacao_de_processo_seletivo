# **Processo Seletivo**
Este projeto simula um processo seletivo onde candidatos são avaliados com base em suas pretensões salariais. O código está dividido em várias funções que realizam diferentes partes do processo.

## **Objetivo do Curso**
Apresentar os conceitos e explorar os tipos de fluxos condicional, excepcional e de repetição em uma aplicação Java.

## **Pré-requisitos**
JDK instalado
IDE escolhida
Noções de Java Sintaxe

## **Assuntos**
Estruturas condicionais: ```if-else```, ```switch-case```
Estruturas de repetição: ```for```, ```while```, ```do-while```
Estruturas de exceções: ```try-catch-finally```, ```throw```

## **Estrutura do Código**
### 1. Classe Principal (`ProcessoSeletivo`)
Contém o método ```main``` que inicia o processo de seleção.
Define uma lista de candidatos.

### 2. Método `main`
Inicializa um array de candidatos.
Chama o método ```selecionarAteCincoCandidatosPorSalarioPretendido``` para iniciar o processo de seleção.

### 3. Método `valorPretendido`
Gera um valor aleatório de pretensão salarial entre 1800 e 2200 usando ```ThreadLocalRandom```.

### 4. Método `selecionarCandidatoPorSalarioPretendido`
Avalia um candidato individualmente com base na sua pretensão salarial.
Compara a pretensão salarial com um salário base de 2000.
Imprime uma mensagem dependendo do resultado da comparação:
Se a pretensão for menor que o salário base, imprime “LIGAR PARA O(A) CANDIDATO(A)”.
Se for igual, imprime “LIGAR PARA O(A) CANDIDATO(A), COM CONTRA PROPOSTA”.
Se for maior, imprime “AGUARDANDO RESULTADO DOS DEMAIS CANDIDATOS”.

### 5. Método `selecionarAteCincoCandidatosPorSalarioPretendido`
Seleciona até cinco candidatos cuja pretensão salarial seja menor ou igual ao salário base.
Chama o método ```tentarLigarParaCandidato``` para tentar contato com o candidato selecionado.

### 6. Método `atendeu`
Simula a tentativa de contato com o candidato, retornando um valor booleano aleatório.

### 7. Método `tentarLigarParaCandidato`
Tenta ligar para o candidato até três vezes.
Se o candidato atender, imprime “CONSEGUIMOS CONTATO COM [candidato] APÓS [tentativas] TENTATIVAS”.
Se não atender após três tentativas, imprime “NÃO CONSEGUIMOS CONTATO COM O(A) CANDIDATO(A) [candidato]”.

## Exemplo de Uso
Para executar o código, basta rodar a classe ```ProcessoSeletivo```. O programa irá simular o processo de seleção e tentará ligar para os candidatos selecionados com base em suas pretensões salariais.
