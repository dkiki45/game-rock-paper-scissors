# JOGO-PEDRA-PAPEL-TESOURA
## Como Executar o Jogo

1. **Pré-requisitos:**
   - O Python precisa estar instalado na sua máquina. Caso não tenha, faça o download [aqui](https://www.python.org/downloads/).
   - Certifique-se de ter o Python 3.x.

2. **Executando o Jogo:**
   - Abra o terminal (ou prompt de comando).
   - Navegue até a pasta onde o arquivo `pedra_papel_tesoura.py` está localizado.
   - Execute o comando:
     ```bash
     python pedra_papel_tesoura.py
     ```

   - O jogo irá iniciar e solicitará o nome dos jogadores e o modo de jogo.

## Funcionalidades Implementadas

- **Escolha de Modo de Jogo:**
  O jogo possui dois modos:
  1. **Jogador vs Computador:** O jogador compete contra o computador.
  2. **Jogador vs Jogador:** Dois jogadores podem jogar entre si.

- **Escolha de Jogada:**
  O jogador pode escolher entre três opções: Pedra, Papel ou Tesoura. A escolha é feita através de números:
  - 1: Pedra
  - 2: Papel
  - 3: Tesoura

- **Determinação do Vencedor:**
  - Pedra vence Tesoura.
  - Tesoura vence Papel.
  - Papel vence Pedra.

- **Placar e Histórico:**
  O jogo mantém o placar de vitórias de cada jogador e o número de empates.
  Também armazena o histórico das partidas jogadas.

- **Opção para Jogar Novamente:**
  O jogo permite que o usuário decida se quer jogar novamente após cada rodada.

- **Tratamento de Erros:**
  O código garante que o jogador só insira opções válidas (1, 2 ou 3) para as jogadas.

## Conceitos de Python Aplicados

- **Funções:** 
  - A lógica do jogo foi dividida em funções para organizar melhor o código. 
  - Exemplo: `obter_escolha_jogador()` e `determinar_vencedor()` são funções que recebem parâmetros e retornam valores, facilitando a reutilização do código.

- **Estruturas Condicionais:**
  - `if`, `elif`, e `else` foram usados para determinar o vencedor de cada rodada e para verificar as opções de jogada válidas.

- **Laços de Repetição:**
  - O jogo usa o `while` para permitir várias rodadas até que o jogador escolha sair.

- **Entrada de Dados:**
  - A função `input()` foi usada para capturar as escolhas dos jogadores, como o nome e as jogadas (Pedra, Papel ou Tesoura).

- **Função `random.choice()`:**
  - O computador escolhe uma jogada aleatória usando a função `random.choice()` para simular uma escolha de jogada no modo "Jogador vs Computador".

- **Listas:**
  - O histórico das partidas é armazenado em uma lista, permitindo que o jogador veja todas as rodadas anteriores.

- **String Manipulation:**
  - O código manipula e exibe strings de forma a mostrar o nome dos jogadores, as jogadas e o resultado da rodada de forma clara.

- **Laços de repetição e manipulação de strings para controle do fluxo do jogo:**
  - O jogo utiliza o laço `while` para garantir que o jogo continue até o jogador decidir parar.

## Observações Finais

Esse projeto foi desenvolvido como parte do aprendizado dos conceitos fundamentais de programação em Python, como controle de fluxo, funções e manipulação de dados do usuário. Ele pode ser facilmente expandido com novos recursos, como um sistema de pontuação mais complexo ou modos de jogo adicionais.
