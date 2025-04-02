# Jogo de Pedra, Papel e Tesoura

Bem-vindo ao repositório do **Jogo de Pedra, Papel e Tesoura**! Este é um jogo simples desenvolvido em **Python**, onde o jogador pode desafiar outro jogador ou o computador em uma partida de **Pedra, Papel e Tesoura**. O jogo mantém um histórico de partidas, apresenta o placar final e permite que o usuário jogue várias rodadas.

## Sumário

- [Sobre o Jogo](#sobre-o-jogo)
- [Como Jogar](#como-jogar)
  - [Requisitos](#requisitos)
  - [Instruções para Jogar](#instruções-para-jogar)
  - [Como Rodar o Jogo](#como-rodar-o-jogo)
  - [Estrutura do Código](#estrutura-do-código)
- [Exemplo de Execução](#exemplo-de-execução)

## Sobre o Jogo

O **Jogo de Pedra, Papel e Tesoura** permite que dois jogadores ou um jogador contra o computador joguem partidas de acordo com as regras clássicas. O jogo exibe um placar dinâmico, informa o vencedor de cada rodada e permite ao usuário jogar várias rodadas seguidas. Ele também mantém um **histórico das partidas** jogadas.

O jogo é baseado nas seguintes regras:

- Pedra vence Tesoura
- Tesoura vence Papel
- Papel vence Pedra

## Como Jogar

### Requisitos

Para jogar, você precisará de:

- **Python 3.x** instalado no seu computador.
- Nenhuma biblioteca externa é necessária, o jogo utiliza a biblioteca `random` que já vem com o Python.

### Instruções para Jogar

1. **Inicialização:**
   - O jogo começa com uma mensagem de boas-vindas.
   - O jogador 1 deve informar seu nome.
   - O jogo então perguntará qual o modo de jogo:
     - **1** para jogar contra o **Computador**.
     - **2** para jogar contra outro **Jogador**.

2. **Escolha de Jogada:**
   - O jogador escolhe entre as opções:
     - **1** para **Pedra**.
     - **2** para **Papel**.
     - **3** para **Tesoura**.
   - O computador faz uma escolha aleatória, caso o jogador esteja jogando contra ele.

3. **Resultado da Rodada:**
   - O vencedor da rodada será determinado com base nas regras clássicas:
     - Pedra vence Tesoura.
     - Tesoura vence Papel.
     - Papel vence Pedra.
   - Se ambos escolherem a mesma jogada, é um **empate**.

4. **Continuar Jogando:**
   - Após cada rodada, o jogo pergunta se o jogador quer jogar novamente. Se sim, a rodada recomeça. Caso contrário, o jogo é finalizado e o placar final é mostrado.

5. **Placar Final:**
   - O histórico das partidas e o placar de vitórias são exibidos no final.

### Como Rodar o Jogo

Para jogar, siga as etapas abaixo:

1. Clone ou baixe este repositório para o seu computador.
2. Abra o terminal ou prompt de comando e navegue até o diretório onde o código foi baixado.
3. Execute o arquivo Python com o comando:

   ```bash
   python pedra_papel_tesoura.py
   
4. Siga as instruções exibidas na tela para jogar.

### Estrutura do código

1. **Módulo random**
   - Utilizado para permitir que o computador escolha aleatoriamente entre Pedra, Papel ou Tesoura no modo "Jogador vs Computador".

2. **Entrada e Validação de Dados**
   - O uso da função input() permite capturar as escolhas dos jogadores e validar as entradas com estruturas de repetição while.

3. **Dicionários**
   - As opções de jogada são armazenadas em um dicionário opcoes para facilitar a conversão entre entrada numérica e escolha textual.

5. **Laços de Repetição**
   - O jogo utiliza while para garantir a repetição do fluxo até que o jogador decida encerrar.

6. **Estruturas Condicionais**
   - if, elif e else são usados para validar entradas, determinar o vencedor e controlar o fluxo do jogo.

7. **Manipulação de Strings**
   - O código exibe mensagens formatadas com interpolação de strings para melhorar a experiência do usuário.

8. **Listas**
   - O histórico das partidas é armazenado em uma lista para manter um registro das jogadas anteriores.

9. **Dicionários para Controle de Placar**
    - O placar é armazenado em um dicionário, permitindo fácil atualização e exibição do número de vitórias e empates.
  
## Exemplo de Execução

   ```bash
   Bem-vindo ao Jogo de Pedra, Papel e Tesoura!
   Nome do Jogador 1: João
   Escolha o modo: 
   (1) vs Computador 
   (2) vs Jogador
    1

   Nova Rodada!
   
   João, escolha sua jogada: 
   [1] Pedra 
   [2] Papel 
   [3] Tesoura 
   Escolha: 1
   
   Computador escolheu: Tesoura
   
   João escolheu: Pedra
   Computador escolheu: Tesoura
   
   Jogador 1 venceu esta rodada!
   
   Deseja jogar novamente? (s/n): n
   
   Histórico de Partidas:
   João (Pedra) vs Computador (Tesoura) → Jogador 1 venceu
   
   Placar Final:
   João: 1 vitórias
   Computador: 0 vitórias
   Empates: 0
   Obrigado por jogar! Até a próxima!

