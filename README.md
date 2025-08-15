# codesoft
TO-DO  project
import tkinter as tk

def add_task():
    task = entry.get()
    if task != "":
        listbox.insert(tk.END, task)
        entry.delete(0, tk.END)

root = tk.Tk()
root.title("To-Do List")

entry = tk.Entry(root, width=40)
entry.pack(pady=10)

add_btn = tk.Button(root, text="Add Task", command=add_task)
add_btn.pack()

listbox = tk.Listbox(root, width=50)
listbox.pack(pady=10)

root.mainloop()
