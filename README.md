# Trignometric_table

from tkinter import *
t=Tk()
t.geometry("222x333")
t.configure(bg="black")
t.title("Trigonometric")
def go():

    f=e.get()
    
    e.delete(0,END)#to delete what ever written there like sin30
    if f=='sin30':
        evar.set(e.get()+"1/2")
    elif f=='sin45':
        evar.set(e.get()+"1/√2")
    elif f=="sin60":
        evar.set(e.get()+"√3/2")
    elif f=="sin90":
        evar.set(evar.get()+"1")
    elif f=="sin0":
        evar.set(evar.get()+"0")
    elif f=="sin90":
        evar.set(evar.get()+"1")

        
    elif f=='cos30':
        evar.set(e.get()+"√3/2")
    elif f=='cos45':
        evar.set(e.get()+"1/√2")
    elif f=="cos60":
        evar.set(e.get()+"1/2")
    elif f=="cos90":
        evar.set(evar.get()+"0")
    elif f=="cos0":
        evar.set(evar.get()+"1")
     
    elif f=='tan30':
        evar.set(e.get()+"√3/3")
    elif f=='tan45':
        evar.set(e.get()+"1")
    elif f=="tan60":
        evar.set(e.get()+"√3")
    elif f=="tan90":
        evar.set(evar.get()+"Not Define")
    elif f=="tan0":
        evar.set(evar.get()+"0")
        
    elif f=='cosec30':
        evar.set(e.get()+"2")
    elif f=='cosec45':
        evar.set(e.get()+"√2")
    elif f=="cosec60":
        evar.set(e.get()+"2√3/3")
    elif f=="cosec90":
        evar.set(evar.get()+"1")
    elif f=="cosec0":
        evar.set(evar.get()+"Not Define")
        
        
    elif f=='sec30':
        evar.set(e.get()+"2√3/3")
    elif f=='sec45':
        evar.set(e.get()+"√2")
    elif f=="sec60":
        evar.set(e.get()+"2")
    elif f=="sec90":
        evar.set(evar.get()+"Not Define")
    elif f=="sec0":
        evar.set(evar.get()+"1")
        
        
    elif f=='cot30':
        evar.set(e.get()+"√3")
    elif f=='cot45':
        evar.set(e.get()+"1")
    elif f=="cot60":
        evar.set(e.get()+"√3/3")
    elif f=="cot90":
        evar.set(evar.get()+"0")
    elif f=="cot0":
        evar.set(evar.get()+"Not Define")
        
        
        
        
        
        
    
    
    
    
        
        
        
        
def sin():
    e.delete(0,END)
    evar.set(evar.get()+"sin")
def cos():
    e.delete(0,END)
    evar.set(evar.get()+"cos")
def tan():
    e.delete(0,END)
    evar.set(evar.get()+"tan")
def cosec():
    e.delete(0,END)
    evar.set(evar.get()+"cosec")
def sec():
    e.delete(0,END)
    evar.set(evar.get()+"sec")
def cot():
    e.delete(0,END)
    evar.set(evar.get()+"cot")
    
    
    
    
    
    
    
def t3():
    evar.set(evar.get()+"30")   
def f4():
    evar.set(evar.get()+"45") 
def s6():
    evar.set(evar.get()+"60") 
def z0():
    evar.set(evar.get()+"0") 
def n9():
    evar.set(evar.get()+"90")    

    
    
def delete():
    e.delete(0,END)
    
    
    
evar=StringVar()
e=Entry(textvariable=evar,font=("",33))
e.place(x=0,y=0,width=222,height=70)

b=Button(text="30",font=("",28),command=t3,bg='grey',fg='white')
b.place(x=10,y=90,width=44,height=39)
b=Button(text="45",command=f4,font=("",28),bg='grey',fg='white')
b.place(x=85,y=90,width=44,height=39)
b=Button(text="60",command=s6,font=("",28),bg='grey',fg='white')
b.place(x=160,y=90,width=44,height=39)

b=Button(text="0",command=z0,font=("",28),bg='grey',fg='white')
b.place(x=45,y=130,width=44,height=39)
b=Button(text="90",command=n9,font=("",28),bg='grey',fg='white')
b.place(x=130,y=130,width=44,height=39)






# b=Button(text="click",command=go)
# b.place(x=90,y=90)

b=Button(text="Sin",command=sin,font=("",26),bg='blue',fg='white')
b.place(x=5,y=200,width=64,height=49)
b=Button(text="Cos",command=cos,font=("",26),bg='blue',fg='white')
b.place(x=85,y=200,width=64,height=49)
b=Button(text="tan",command=tan,font=("",26),bg='blue',fg='white')
b.place(x=160,y=200,width=64,height=49)
b=Button(text="Cosec",command=cosec,font=("",16,'bold'),bg='blue',fg='white')
b.place(x=5,y=260,width=69,height=49)
b=Button(text="Sec",command=sec,font=("",26),bg='blue',fg='white')
b.place(x=85,y=260,width=64,height=49)
b=Button(text="Cot",comman=cot,font=("",26),bg='blue',fg='white')
b.place(x=160,y=260,width=64,height=49)

b=Button(text="ans",command=go,font=("",16),bg='green',fg='white')
b.place(x=5,y=172,width=110,height=26)
b=Button(text="Delete",command=delete,font=("",16),bg='red',fg='white')
b.place(x=120,y=172,width=110,height=26)



t.mainloop()
