# Exercicio044.py


preco = float(input('Preço das compras: '))
print('''FORMAS DE PAGAMENTO
[ 1 ] Dinheiro/Cheque
[ 2 ] Pix
[ 3 ] Debito
[ 4 ] Credito
''')
opcao = int(input('Digite sua opção: '))
if opcao == 1:
    total = preco - (preco * 5 / 100)
elif opcao == 2:
    total = preco - (preco * 10 / 100)
elif opcao == 4:
    total = preco + (preco * 20 / 100)
    tot = int(input('Quantas parcelas: '))
    parcela = total / tot
    print(( 'sua compra sera parcelada em {}  de {} com juros'.format(tot,parcela)))
print('Sua compra de {} vai custar {} no final.'.format(preco,total))
