import string
import random

def gerarsenha(tamanho=8):
    caracteres = string.ascii_letters + string.digits + string.punctuation
    senha = ''.join(random.choice(caracteres) for _ in range(tamanho))
    return senha

senhaforte=gerarsenha()
print("A tua senha é:", senhaforte)

print(string.ascii_letters + string.digits + string.punctuation)
