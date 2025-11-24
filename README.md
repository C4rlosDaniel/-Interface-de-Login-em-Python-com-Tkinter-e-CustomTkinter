# 🖥️ Interface de Login em Python com Tkinter e CustomTkinter

Este repositório apresenta um exemplo simples e moderno de interface gráfica (GUI) criada em Python utilizando **Tkinter** e sua versão estilizada **CustomTkinter**.  
O projeto demonstra como criar uma janela de login funcional com tema escuro, campos de entrada, checkbox e botão com ação.

---

## 🚀 Funcionalidades

- Interface gráfica criada com Tkinter e CustomTkinter  
- Tema escuro aplicado automaticamente  
- Campo de e-mail  
- Campo de senha com ocultação (`show='*'`)  
- Opção “Lembrar Login”  
- Botão com função callback  
- Estrutura simples, ideal para iniciantes em GUI com Python

---

## 🧩 Tecnologias Utilizadas

- **Python 3.x**
- **Tkinter** (biblioteca nativa do Python)
- **CustomTkinter** (interface moderna e estilizada)

---

## 📦 Instalação

Antes de executar, instale a dependência necessária:

```bash
pip install customtkinter
```

---

## ▶️ Como Executar

Basta rodar o arquivo Python:

```bash
python nome_do_arquivo.py
```

---

## 🧠 Código Utilizado

```python
import tkinter

janela = tkinter.Tk()
janela.geometry("500x300")


def clique():
    print("Fazer Login")

texto = tkinter.Label(janela, text='Fazer Login')
texto.pack(padx=10, pady=10)

botao = tkinter.Button(janela, text="Login", command=clique)
botao.pack(padx=10, pady=10)

janela.mainloop()


import customtkinter

customtkinter.set_appearance_mode("dark")
customtkinter.set_default_color_theme('dark-blue')

janela = customtkinter.CTk()
janela.geometry('500x300')


def clique():
    print("Fazer Login")

texto = customtkinter.CTkLabel(janela, text='Fazer Login')
texto.pack(padx=10, pady=10)

email = customtkinter.CTkEntry(janela, placeholder_text="Seu e-mail")
email.pack(padx=10, pady=10)

senha = customtkinter.CTkEntry(janela, placeholder_text="Sua Senha", show='*')
senha.pack(padx=10, pady=10)

checkbox = customtkinter.CTkCheckBox(janela, text="Lembrar Login")
checkbox.pack(padx=10, pady=10)

botao = customtkinter.CTkButton(janela, text="Login", command=clique)
botao.pack(padx=10, pady=10)

janela.mainloop()
```

---

## 📚 Objetivo Educacional

Este projeto serve como base para quem deseja aprender a criar interfaces gráficas em Python e evoluir para aplicações mais completas, como sistemas de autenticação, dashboards e ferramentas desktop.

---
