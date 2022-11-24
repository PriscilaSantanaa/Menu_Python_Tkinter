# Menu_Python_Tkinter
Menu feito para a matéria de linguagem de programação 2 utilizando a tabela do Tkinter. 

```
from tkinter import *

root = Tk()

class Application():
    def __init__(self):
        self.root = root
        self.tela()
        self.div_tela()
        self.criando_botoes()
        root.mainloop()

    def tela(self):
       self.root.title("Star saudável") #Definindo nome da janela
       self.root.configure(background='White') #Definindo cor de fundo
       self.root.geometry("700x500") #Configurando tamanho da janela
       self.root.resizable(True, True) #Permitindo redimensionar a janela 
       self.root.maxsize(width=988, height=788) #Limitando o maior tamanho da janela
       self.root.minsize(width= 500, height= 400)

    def div_tela(self):
        self.frame_1 = Frame(self.root, bd = 4, bg = "LightSteelBlue", highlightbackground= "LightPink", highlightthickness= 3)
        self.frame_1.place(relx = 0.1, rely= 0.06, relwidth= 0.8, relheight= 0.4) #0 esquerdo, 1 direito
        self.frame_2 = Frame(self.root, bd = 4, bg = "LightSteelBlue", highlightbackground= "LightPink", highlightthickness= 3)
        self.frame_2.place(relx = 0.1, rely= 0.5, relwidth= 0.8, relheight= 0.4) #0 esquerdo, 1 direito

    def criando_botoes(self):
        #Criando botão cadastrar
        self.bt_limpar = Button(self.frame_1, text="Novo")
        self.bt_limpar.place(relx= 0.2, rely= 0.1, relwidth= 0.1, relheight= 0.15)

        #Criando botão buscar
        self.bt_limpar = Button(self.frame_1, text="Buscar")
        self.bt_limpar.place(relx= 0.35, rely= 0.1, relwidth= 0.1, relheight= 0.15)

        #Criando botão apagar
        self.bt_limpar = Button(self.frame_1, text="Apagar")
        self.bt_limpar.place(relx= 0.6, rely= 0.1, relwidth= 0.1, relheight= 0.15)

        #Criando botão alterar
        self.bt_limpar = Button(self.frame_1, text="Alterar")
        self.bt_limpar.place(relx= 0.7, rely= 0.1, relwidth= 0.1, relheight= 0.15)

        #Criando botão limpar
        self.bt_limpar = Button(self.frame_1, text="Limpar")
        self.bt_limpar.place(relx= 0.8, rely= 0.1, relwidth= 0.1, relheight= 0.15)

        #Criação de label para colocar ID_Cliente e ID_Médico
        self.lb_nome = Label(self.frame_1, text="ID")
        self.lb_nome.place(relx= 0.05, rely= 0.05)

        self.nome_entry = Entry(self.frame_1)
        self.nome_entry.place(relx = 0.05, rely= 0.2, relwidth= 0.07)

        #Criando label para colocar nome
        self.lb_nome = Label(self.frame_1, text="Nome")
        self.lb_nome.place(relx= 0.05, rely= 0.35)

        self.nome_entry = Entry(self.frame_1)
        self.nome_entry.place(relx = 0.05, rely= 0.5, relwidth= 0.9)

Application()

´´´
