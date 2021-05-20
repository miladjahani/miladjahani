#Made by Mr. B _ A _ B _ A  ( group 12 computer )
from tkinter import *
from tkinter import messagebox
#########################################################################################################################
listAlf = ['abcdefghijklmnopqrstuvwxyzabcdefghijklmnopqrstuvwxyz']
t = Tk()
t.geometry('500x400')
t.title('Cryptotion')
t.resizable(False, False)
t.configure(bg='#ffdd00')
#######################################################################################################################
def main_exit():
    rr = messagebox.askyesnocancel('Notification', 'Are you sure you want to get out of the Cryptotion ?', parent=t)
    if rr:
        t.destroy()


btn2 = Button(t, text='Exit', bd=10, bg='#ff0000', fg='#0affff', activebackground='#ff1e1e', width=10,
              font=('times', 15, 'italic bold'),
              command=main_exit)
btn2.place(x=415, y=345, width=80, height=50)
###########################################################################################################################
def on_enterbtn2(e):
    btn2['bg'] = '#ff1e1e'


def on_leavebtn2(e):
    btn2['bg'] = '#ff0000'

def on_enterh(e):
    h['bg'] = '#2846ff'


def on_leaveh(e):
    h['bg'] = '#0a2bff'


def on_enterd(e):
    d['bg'] = '#2846ff'


def on_leaved(e):
    d['bg'] = '#0a2bff'
#########################################################################################################################
def fh():
    k = Tk()      
    k.geometry('500x400')
    k.title('Cryptography')
    k.resizable(False, False)
    k.configure(bg='#3bff14')
    i = Entry(k)
    i.place(x=110, y=50, width=250, height=30)

    def cryptoghraphy(i, w):
        finaly = ""
        for io in range(len(i)):
            final1 = djd[io]
            for q in range(26):
                if final1 == listAlf[q]:
                    finaly += listAlf[q + w]
            if final1 == " ":
                finaly += " "
        return finaly

    def clickcripto():
        bo1 = i.get()
        bo2 = int(aaaa.get())
   
        djd.config(text=cryptoghraphy(bo1, bo2))
        i.delete(0, 'end')
        aaaa.delete(0, 'end')
    
    i = Entry(k)
    i.place(x=110, y=50, width=250, height=30)
    aaaa = Entry(k)
    aaaa.place(x=115, y=124, width=50, height=30)

    bbbb = Label(k, text="Enter Factor  >>>", bg='#3bff14', fg='#da1eff', font=('times', 10, 'italic bold'))
    bbbb.place(x=0, y=116, width=115, height=50)
    djd = Label(k, bg='white', fg='black', font=('times', 10, 'italic bold'))
    djd.place(x=70, y=200, width=350, height=100)

    btgj = Button(k, text='Start', bd=10, bg='#da1eff', fg='#3bff14', activebackground='#e65aff', width=10,
                  font=('times', 15, 'italic bold'), command=clickcripto)
    btgj.place(x=170, y=110)

    def main_exit1():
        rr = messagebox.askyesnocancel('Notification', 'Are you sure you want to get out of the Cryptography ?',
                                       parent=k)
        if rr:
            k.destroy()

    btn22 = Button(k, text='Exit', bd=10, bg='#ff0000', fg='#0affff', activebackground='#ff1e1e', width=10,
                   font=('times', 15, 'italic bold'),
                   command=main_exit1)
    btn22.place(x=415, y=345, width=80, height=50)

    def on_enterbtgj(e):
        btgj['bg'] = '#e65aff'


    def on_leavebtgj(e):
        btgj['bg'] = '#da1eff'
        
    def on_enterbtn22(e):
        btn22['bg'] = '#ff1e1e'


    def on_leavebtn22(e):
        btn22['bg'] = '#ff0000'
        
    btgj.bind('<Enter>',on_enterbtgj)
    btgj.bind('<Leave>',on_leavebtgj)

    btn22.bind('<Enter>',on_enterbtn22)
    btn22.bind('<Leave>',on_leavebtn22)

    bbb = Label(k, text="<<<", bg='#3bff14', fg='#da1eff', font=('times', 15, 'italic bold'))
    bbb.place(x=380, y=43, width=50, height=50)



    
    k.mainloop()
##########################################################################################################################

def fg():
    o = Tk()
    o.geometry('500x400')
    o.title('Decryption')
    o.resizable(False, False)
    o.configure(bg='#3bff14')
    ih = Entry(o)
    ih.place(x=110, y=50, width=250, height=30)
    aaaaa = Entry(o)
    aaaaa.place(x=115, y=124, width=50, height=30)
    bbbbb = Label(o, text="Enter Factor  >>>", bg='#3bff14', fg='#da1eff', font=('times', 10, 'italic bold'))
    bbbbb.place(x=0, y=116, width=115, height=50)
    djdd = Text(o)
    djdd.place(x=70, y=200, width=350, height=100)

    btgjb = Button(o, text='Start', bd=10, bg='#da1eff', fg='#3bff14', activebackground='#e65aff', width=10,
                   font=('times', 15, 'italic bold'))
    btgjb.place(x=170, y=110)

    def main_exit2():
        rr = messagebox.askyesnocancel('Notification', 'Are you sure you want to get out of the Decryption ?', parent=o)
        if rr:
            o.destroy()

    btn222 = Button(o, text='Exit', bd=10, bg='#ff0000', fg='#0affff', activebackground='#ff1e1e', width=10,
                   font=('times', 15, 'italic bold'),
                   command=main_exit2)
    btn222.place(x=415, y=345, width=80, height=50)

    def on_enterbtgjb(e):
        btgjb['bg'] = '#e65aff'


    def on_leavebtgjb(e):
        btgjb['bg'] = '#da1eff'
        
    def on_enterbtn222(e):
        btn222['bg'] = '#ff1e1e'


    def on_leavebtn222(e):
        btn222['bg'] = '#ff0000'
        
    btgjb.bind('<Enter>',on_enterbtgjb)
    btgjb.bind('<Leave>',on_leavebtgjb)

    btn222.bind('<Enter>',on_enterbtn222)
    btn222.bind('<Leave>',on_leavebtn222)

    bbbb = Label(o, text="<<<", bg='#3bff14', fg='#da1eff', font=('times', 15, 'italic bold'))
    bbbb.place(x=380, y=43, width=50, height=50)

    o.mainloop()
##############################################################################################################################

d = Button(t, text='Cryptography', bd=10, bg='#0a2bff', fg='#ffdc00', activebackground='#2846ff', width=10,
           font=('times', 15, 'italic bold'),
           command=fh)
d.place(x=200, y=100, width=150, height=60)

h = Button(t, text='Decryption', bd=10, bg='#0a2bff', fg='#ffdc00', activebackground='#2846ff', width=10,
           font=('times', 15, 'italic bold'),
           command=fg)
h.place(x=200, y=200, width=150, height=60)
############################################################################################################
b = Label(t, text="Please select one of", bg='#ffdd00', fg='#0a2bff', font=('times', 15, 'italic bold'))
b.place(x=-18, y=150, width=210, height=50)

cc = Label(t, text="Made by Mr. B _ A _ B _ A  ( group 12 computer )", bg='#ffdd00', fg='#0a2bff',
           font=('times', 12, 'italic bold'))
cc.place(x=-26, y=360, width=400, height=50)
##############################################################################################################

h.bind('<Enter>',on_enterh)
h.bind('<Leave>',on_leaveh)

d.bind('<Enter>',on_enterd)
d.bind('<Leave>',on_leaved)

btn2.bind('<Enter>',on_enterbtn2)
btn2.bind('<Leave>',on_leavebtn2)
#############################################################################################################

t.mainloop()
