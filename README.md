# projeto_bompet
import os

def processar_duvidas(resposta, nome):
        print(f'{os.linesep}{nome} Qual seria sua dúvida?{os.linesep}[2] Saber mais sobre a loja{os.linesep}[3] Fale com atendente')
if 
def processarSegundaResposta(resposta, nome):
    if resposta == '1':
        print(f'{os.linesep}{nome} Escolha sua forma de pagamento{os.linesep}[1] Crédito{os.linesep}[2] Boleto Bancario')
    elif resposta == '2':
        print(f'{os.linesep}{nome} Escolha sua forma de pagamento{os.linesep}[1] Crédito{os.linesep}[2] Boleto Bancario')
    elif resposta == '3':
        print(f'{os.linesep}{nome} Escolha sua forma de pagamento{os.linesep}[1] Crédito{os.linesep}[2] Boleto Bancario')
    else:
        print('Digite apenas 1, 2 ou 3')


def solicitar_compra(resposta, nome):
    if resposta == '1':
        print(f'{os.linesep}{nome} Qual produto você deseja comprar?{os.linesep}[1] Saquinho biodegradavel{os.linesep}[2] Suporte {os.linesep}[3] Bombina')
    elif resposta == '2':
        print(f'{os.linesep}{nome} Qual sua dúvida?{os.linesep}')
    else:
        print('Digite apenas 1, ou 2')


def start():
    # Apresentar o chatbot
    print(f'Olá! Bem-vindo ao Bom Pet!{os.linesep}Ao prosseguir com a conversa, você concorda com a nossa comunicação através deste canal, nos termos da Lei 13.709/2018?')
    # pedir o nome
    nome = input('Digite seu primeiro nome: ')
    # pedir o CPF
    cpf = input('Digite seu CPF: ')
    # Oferer o menu de opções
    resposta = input(
        f'O que gostaria de fazer aqui?{os.linesep}[1] - Solicitar uma compra{os.linesep}[2] - Dúvidas{os.linesep}[3] - Orientações{os.linesep}[4] - Informações sobre o prazo{os.linesep}[5] - Endereço{os.linesep}')
    # Processar a resposta enviada

    if resposta == '1':
        solicitar_compra(resposta, nome)
    elif resposta == '2':
        processarSegundaResposta(resposta, nome)
    else:
        print('Número inválido, digite novamente')

if __name__ == '__main__':
    start()
