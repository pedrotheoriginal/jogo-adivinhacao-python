# Jogo de Adivinhação em Python 🎯

Projeto desenvolvido com o objetivo de praticar conceitos fundamentais de lógica de programação em Python, como controlo de fluxo, loops de repetição (`while`), condicionais (`if/elif/else`), geração de números aleatórios e tratamento básico de erros (`try/except`).

## 🎮 Sobre o Jogo

Neste jogo clássico, o computador escolhe um número secreto aleatório entre 1 e 200. O objetivo do jogador é descobrir qual é esse número com o menor número de tentativas possível. A cada palpite incorreto, o programa dá uma dica informando se o número secreto é maior ou menor do que o valor digitado.

## 🚀 Funcionalidades

* **Geração Aleatória:** O número secreto muda a cada partida usando a biblioteca nativa `random`.
* **Contador de Tentativas:** O sistema regista quantas tentativas precisaste para acertar.
* **Tratamento de Erros:** O programa protege contra entradas inválidas (caso o utilizador digite texto em vez de números) sem fechar abruptamente.
* **Menu de Recomeço:** Ao acertar, o jogador pode escolher se deseja iniciar uma nova rodada ou encerrar o jogo.

## 🛠️ Tecnologias Utilizadas
* **Python 3.x** (Conceitos aplicados: Funções, Loops, Condicionais, Tratamento de Exceções e módulo `random`).

## 💻 Exemplo de Código em Destaque

Uma amostra da função principal, mostrando o tratamento de erros e a lógica de tentativas:

```python
import random

def jogar_adivinhacao():
    print("--- Bem-vindo ao jogo de Adivinhação! ---")
    print("Tente adivinhar o número secreto que está entre 1 e 200!\n")

    while True:
        numero_secreto = random.randint(1, 200)
        tentativas = 0

        while True:
            try:
                palpite = int(input("Digite seu palpite: "))
                tentativas += 1
            except ValueError:
                print("Por favor, digite apenas números inteiros válidos.")
                continue

            if palpite < numero_secreto:
                print("Muito baixo! Tente novamente.\n")
            elif palpite > numero_secreto:
                print("Muito alto! Tente novamente.\n")
            else:
                print(f"🎉 Parabéns! Você acertou o número secreto {numero_secreto} em {tentativas} tentativas!\n")
                break
        break
