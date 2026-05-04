# casa
senha_correta = ["123456", "654321", "111111", "222222"]

while True:
    senha_usuario = input("Digite uma senha (somente numeros): ")
    print(f"Senha digitada: {senha_usuario}")
    
    try:
        senha = int(senha_usuario) 
        
    except ValueError as e:
            print("Ocorreu um erro ao ler a senha. Tente novamente.")
    if senha_usuario in senha_correta:
            print(f"Senha '{senha_usuario}' está correta! Acesso liberado!")     
            break
    else:
            print("Senha incorreta! Tente novamente.")
