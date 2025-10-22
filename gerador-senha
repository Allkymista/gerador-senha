import random
import string

def gerar_senha(tamanho=12, usar_maiusculas=True, usar_numeros=True, usar_simbolos=True):
    caracteres = string.ascii_lowercase
    if usar_maiusculas:
        caracteres += string.ascii_uppercase
    if usar_numeros:
        caracteres += string.digits
    if usar_simbolos:
        caracteres += string.punctuation

    senha = ''.join(random.choice(caracteres) for _ in range(tamanho))
    return senha

if __name__ == "__main__":
    print("Gerador de Senhas Seguras 🔐")
    tamanho = int(input("Digite o tamanho da senha: "))
    usar_maiusculas = input("Usar letras maiúsculas? (s/n): ").lower() == 's'
    usar_numeros = input("Usar números? (s/n): ").lower() == 's'
    usar_simbolos = input("Usar símbolos? (s/n): ").lower() == 's'

    senha = gerar_senha(tamanho, usar_maiusculas, usar_numeros, usar_simbolos)
    print(f"\nSua senha gerada é:\n{senha}")
