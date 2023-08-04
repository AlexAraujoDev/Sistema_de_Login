"""O sistema de logind deve permir que  novos usuários sejam cadastrados, e que
usuários existentem possam fazer o login. O sistema deve alertar caso a senha e 
login não estejam corretos."""

# O sistema de login deve permir que novos usuários sejam cadastrados 
# O sistema não deve permitir que usuários duplicados sejam cadastrados
# Permitir que usuários existentes possam fazer o login
# O sistema deve alertar caso a senha e logins não estejam corretos

"""
# O sistema de login deve permir que novos usuários sejam cadastrados 
1. Quais são os dados de entrada necessparios ?
    - Usuário, senha
2. O que devo fazer com estes dados ?
    - Eu devo registrar o usuário e senha que foi digitado
3. Quais são as restrições deste problema ?
    - Não devo permitir cadastro de usuários já existentes
4. Qual é o resultado esperado ?
    - Um novo usuário e senha cadastrados
5. Qual é a sequencia de passos necessárias parachegar ao resultado final ?
    - Receber o usuário
    - Receber a senha
    - Verificar se o usuário já existe
    - Caso não exista, cadastrar aquele usuário e senha
"""


resposta = input('[1] - Cadastrar novo usuário [2] - Fazer login: ')
# Armazenando os usuários existentes
informacoes_aleatorias = [1,5,5,5,'Alex']
usuarios = ['carol','amanda','jeff']
senha = ['123456','abcdef','123abc']

if resposta == '1':
    # Recebendo um usuário
    usuario_digitado = input('Digite seu usuário: ')
    if usuario_digitado in usuarios:
        print('Usuário existente')
    else:
        # Recebendo uma senha
        senha_digitada = input('Digite sua senha: ')
        # Caso não exista cadastrar aquele usuário e senha
        usuarios.append(usuario_digitado)
        senha.append(senha_digitada)
elif resposta == '2':
    # Permitir que usuários existentes possam fazer o login
    # Pedir usuário
    usuario_digitado = input('Digite seu usuário: ')
    # Pedir senha
    senha_digitada = input('Digite uma senha: ')
    # Preciso verificar se a senha providenciada para aquela usuário é a mesma senha que está na nossa lista de senhas
    encontrado = False
    for indice, usuario in enumerate(usuarios):
        if usuario_digitado == usuario and senha_digitada == senha[indice]:
            print('Login feito com sucesso')
            encontrado = True
        elif encontrado == False:
            print('usuário ou senha incorreto!')
else:
    print('Digite apenas 1 ou 2')
