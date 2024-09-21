# Gerador_senha
from random import choice
import string

tamanho_da_senha = int(input("Quantos digitos vai na senha:? "))
caracteres = string.ascii_letters + string.digits + string.punctuation
senha_segura = ""
for i in range(tamanho_da_senha):
    senha_segura += choice(caracteres)

print("Sua senha (segura) gerada foi: ",senha_segura)
