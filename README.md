# 02
no firrst
# Увімкнути модуль Tkinter
from tkinter import *

# Створити функцію для обчислення
def calculate():
    result.set(eval(expression.get()))

# Створити головне вікно програми
root = Tk()
root.geometry("250x100")
root.title("Калькулятор")

# Поле введення для запису виразу
expression = Entry(root, width=30)

# Розташувати поля введення і кнопки з опціями
expression.pack(side = TOP, pady = 5)
result = StringVar()
result.set("0")
display = Label(root, textvariable=result, width=30)
display.pack(side = TOP, pady = 5)
button_frame = Frame(root)
button_frame.pack(side = TOP, pady = 5)
Button(button_frame, text="1", width=5, command=lambda: expression.insert(END, "1")).pack(side=LEFT,padx=5)
Button(button_frame, text="2", width=5, command=lambda: expression.insert(END, "2")).pack(side=LEFT,padx=5)
Button(button_frame, text="3", width=5, command=lambda: expression.insert(END, "3")).pack(side=LEFT,padx=5)
Button(button_frame, text="+", width=5, command=lambda: expression.insert(END, "+")).pack(side=LEFT,padx=5)
Button(button_frame, text="4", width=5, command=lambda: expression.insert(END, "4")).pack(side=LEFT,padx=5)
Button(button_frame, text="5", width=5, command=lambda: expression.insert(END, "5")).pack(side=LEFT,padx=5)
Button(button_frame, text="6", width=5, command=lambda: expression.insert(END, "6")).pack(side=LEFT,padx=5)
Button(button_frame, text="-", width=5, command=lambda: expression.insert(END, "-")).pack(side=LEFT,padx=5)
Button(button_frame, text="7", width=5, command=lambda: expression.insert(END, "7")).pack(side=LEFT,padx=5)
Button(button_frame, text="8", width
