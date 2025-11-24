# 🖥️ Interface de Login em Python (Tkinter + CustomTkinter)

Este repositório apresenta uma interface gráfica simples de login desenvolvida em Python, utilizando **Tkinter** e **CustomTkinter** para fornecer uma aparência moderna em tema escuro.  
O projeto inclui campos de e-mail e senha, checkbox de “Lembrar Login” e botão de ação.

---

## 📸 Demonstração

<img width="1329" height="673" alt="image" src="https://github.com/user-attachments/assets/67504f9b-e256-45de-9a18-d679adeee542" />


---

## 🚀 Funcionalidades

- Interface criada com Tkinter e CustomTkinter  
- Tema escuro aplicado automaticamente  
- Campos de entrada estilizados (e-mail e senha)  
- Checkbox para lembrar login  
- Botão com função vinculada  
- Ideal para iniciantes em GUI com Python

---

## 📦 Instalação

Antes de executar, instale a dependência necessária:

```bash
pip install customtkinter
```

---

---

## 🧠 Código Completo

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
