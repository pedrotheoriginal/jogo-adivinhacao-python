#  Jogo de Adivinhação em Python

Projeto desenvolvido com o objetivo de praticar conceitos fundamentais de lógica de programação em Python, como controle de fluxo, loops de repetição (`while`), condicionais (`if/elif/else`), geração de números aleatórios e tratamento básico de erros (`try/except`).

## 🎮 Sobre o Jogo
Neste jogo clássico, o computador escolhe um número secreto aleatório entre **1 e 200**. O objetivo do jogador é descobrir qual é esse número com o menor número de tentativas possível. A cada palpite incorreto, o programa dá uma dica informando se o número secreto é **maior** ou **menor** do que o valor digitado.

## 🚀 Funcionalidades
* **Geração Aleatória:** O número secreto muda a cada partida usando a biblioteca nativa `random`.
* **Contador de Tentativas:** O sistema registra quantas tentativas você precisou para acertar.
* **Tratamento de Erros:** O programa protege contra entradas inválidas (caso o usuário digite texto em vez de números) sem fechar abruptamente.
* **Menu de Recomeço:** Ao acertar, o jogador pode escolher se deseja iniciar uma nova rodada ou encerrar o jogo.

## 🛠️ Tecnologias Utilizadas
* **Python** (Conceitos aplicados: Funções, Loops, Condicionais, Tratamento de Exceções e módulo `random`).

## 💻 Como executar o projeto na sua máquina

1. Certifique-se de ter o Python instalado no seu computador.
2. Clone este repositório ou baixe o arquivo `.py` do jogo.
3. Abra o terminal na pasta onde o arquivo está salvo.
4. Execute o comando:
   ```bash
   python adivinhacao.py
