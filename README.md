Loja de cosméticos - Python

class Produto: def init (self, nome_prod, lote, validade, fornecedor, quantidade): self.nome_prod = nome_prod self.lote = lote self.validade = validade self.fornecedor = fornecedor self.quantidade = quantidade

class LojaCosmetico: def init (self): self.produtos = []

def cadastro_prod(self, nome_prod, lote, validade, fornecedor, quantidade):
    produto = Prod(nome_prod, lote, validade, fornecedor, quantidade)
    self.prod.append(prod)
    print("Olá, seu produto foi cadastrado!")

def buscar_prod(self, nome_prod):
    for produto in self.produtos:
        if prod.nome_prod == nome_prod:
            print("O seu produto foi encontrado:")
            print("Nome:", produto.nome_prod)
            print("Lote:", produto.lote)
            print("Validade:", produto.validade)
            print("Fornecedor:", produto.fornecedor)
            print("Quantidade:", produto.quantidade)
            return
    	print("Produto não encontrado.")

def mostrar_estoque(self):
    	print("Estoque:")
    for produto in self.produtos:
        print("Nome:", produto.nome_prod)
        print("Quantidade:", produto.quantidade)
        print("XXXX")

def registro_venda(self, nome_prod, quantidade):
    for produto in self.produtos:
        if produto.nome_prod == nome:
            if produto.quantidade >= quantidade:
                produto.quantidade -= quantidade
                print("Sua venda foi registrada!")
                return
            else:
                print("O produto buscado não possui estoque. ")
                return
    	print("Produto não encontrado.")

def gerar_relatorio(self):
    	print("Relatório de Estoque:")
    for produto in self.produtos:
        print("Nome:", produto.nome_prod)
        print("Lote:", produto.lote)
        print("Validade:", produto.validade)
        print("Fornecedor:", produto.fornecedor)
        print("Quantidade:", produto.quantidade)
        print("XXXX")
def exibir_menu(): print("=== Menu ===") print("1. Cadastrar Produto") print("2. Buscar Produto") print("3. Exibir Estoque") print("4. Registrar Venda") print("5. Gerar Relatório") print("6. Sair")

controle = LojaCosmeticos()

while True: exibir_menu() opção = input("Selecione uma das opções disponíveis: ")

if opcao == "1":
    nome_prod = input("Informe o nome do produto: ")
    lote = input("Informe o número do lote: ")
    validade = input("Informe a data de validade: ")
    fornecedor = input("Informe o nome do fornecedor: ")
    quantidade = int(input("Informe a quantidade: "))
    controle.cadastrar_produto(nome_prod, lote, validade, fornecedor, quantidade)
    	print()

elif opcao == "2":
    nome = input("Informe o nome do produto: ")
    controle.buscar_produto(nome)
   	print()

elif opcao == "3":
    controle.exibir_estoque()
    	print()

elif opcao == "4":
    nome = input("Informe o nome do produto: ")
    quantidade = int(input("Informe a quantidade vendida: "))
    controle.registrar_venda(nome_prod, quantidade)
    	print()

elif opcao == "5":
    controle.gerar_relatorio()
    	print()

elif opcao == "6":
    	print("O programa será encerrado. ")
    break

else:
   	print("A opção é inválida. Tente novamente.")
    		print()
