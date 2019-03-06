# Volta-pela-Matrix
# Mini jogo criado enquanto eu aprendia bases de programação em Python.
#IDENTIFICAÇÃO
print ('Olá forasteiro. Qual o seu nome?')
nome = input ()

while nome=='':
    print ('Nome, por favor?') #BUG: ISSO SÓ ACONTECE 1 VEZ! DEPOIS VAI PRA else.
    nome = input ()
    if nome == 'Vitor' or nome =='vitor':
           print ('Estávamos esperando por você, Vitor! Bem vindo à Matrix.')
    else:
           print('.')
           print('.')
           print('.')
           print('[checa a lista de convidados com olhar confuso]')
           print('.')
           print('.')
           print('.')
           print('Sua chegada não era esperada, ' + nome)
print ()

#IDADE
print ('Qual a sua idade?')
idade = int(input())
if nome == 'Vitor' or nome == 'vitor' and idade == 30:
    print ('Só pra confirmar, Vitor. Aguarde para tomar a pílula azul.')
elif idade <= 17:
    print ('Você não tem idade para tomar a pílula azul. Adeus.')
elif idade >= 60:
    print ('Woah! Acho melhor não forçarmos esse coração idoso!')
elif idade >= 18:
    print ('Não era para você estar aqui, mas já que tem idade suficiente, poderá seguir por sua conta e risco.')
    print ('Você tem certeza de que quer tomar a pílula azul?')
    print ('[sim] ou [não]')
    resposta = input ()
    if resposta == 'sim' or resposta == 'Sim':
        print ('Então aperte o cinto e lá vamos nós!')
    elif resposta == 'não' or resposta == 'Não':
        print ('acho mais seguro, mesmo. Adeus.')
    else:
        print ('Resposta errada, otário!')
print ()               

#PILOTO
print ('Piloto: Lembre-se que apenas Morfeu pode te levar para além da barreira.')
print () #ADICIONAR ESCOLHAS

#A BARREIRA
print ('[Você chega ao pé da grande barreira de estática. Ela parece intransponível e dá choques quando encosta nela.]')
print ()

#ADICIONAR ESCOLHAS
print ('[A alguns metros existe um portão igual a uma entrada USB gigante. No fundo uma porta possui a palavra "senha" inscrita.]')
print ('[Digite a senha.]')
senha = input ()
while senha != 'Morfeu' or senha != 'morfeu':
    print ('Acesso negado. Tente novamente')
    senha = input ()
    if senha == 'Morfeu' or senha == 'morfeu':
        break
print ('Acesso liberado!')
print ()

#FIM
print ('[A simulação chega ao fim e você acorda]')
print ('Desconecte-se da Matrix')
