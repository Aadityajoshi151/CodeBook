## Python-Tkinter Snippets
### **Boilerplate 🍽️**
```
from tkinter import *
from tkinter import ttk

class ClassName:
#user defined functions will go here
    def __init__(self,app):
        #User defined elements will go here
        self.mybutton = ttk.Button(app,text="Hello World")
        self.mybutton.pack()

def main():
    root = Tk()
    root.title("App Title")
    root.geometry("200x200")
    root.resizable("False","False")
    obj = ClassName(root)
    root.mainloop()

if __name__ == "__main__":
    main()      
```
### **A Button**
```
mybutton = ttk.Button(root,text="Hello World",state=DISABLED,padx=50,pady=50,command=functionname,fg="blue")
mybutton.pack()
```
### **Custom Messagebox**
```
custommessagebox = Toplevel()
custommessagebox.attributes(\"-toolwindow\", True)
'''
removes icon,minimize,maximize buttons from window". It is just a top level window. The content inside the  messagebox is made same as normal tkinter.
'''
```