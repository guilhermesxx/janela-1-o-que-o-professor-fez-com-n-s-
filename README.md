import tkinter as tk


Window = tk.Tk()
Window.title("guimaraes")
Window.geometry("500x500")
Window.configure(background="#4B0082")


nome = tk.Label(Window, text="bom dia")
nome.pack()


txtentrada = tk.Entry(Window)
txtentrada.pack()


def machado_de_assis():
    
    new_window = tk.Toplevel(Window)
    new_window.title("Nova Janela")
    new_window.geometry("300x200")
    new_window.configure(background="#B0E0E6")
    

    inspiracao = txtentrada.get()   
    
    t = tk.Label(new_window, text=inspiracao)
    t.pack()


btn = tk.Button(Window, text="mostrar", command=machado_de_assis)
btn.pack()

Window.mainloop()
