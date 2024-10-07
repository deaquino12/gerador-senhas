# gerador-senhas
 Um gerador de senhas aleatórias.
gerador-senhas/
├── gerador.pyimport random
import string

def gerar_senha(tamanho=12):
    caracteres = string.ascii_letters + string.digits + string.punctuation
    senha = ''.join(random.choice(caracteres) for _ in range(tamanho))
    return senha

if __name__ == "__main__":
    tamanho = int(input("Digite o tamanho da senha: "))
    print("Senha gerada:", gerar_senha(tamanho))

└── README.md# Gerador de Senhas

Um gerador de senhas aleatórias em Python.

## Como usar

1. Clone o repositório.
2. Execute o script `gerador.py`.
3. Insira o tamanho da senha que deseja gerar.

## Dependências

Nenhuma dependência externa é necessária.
git add .
git commit -m "Adiciona gerador de senhas"
git push origin main

