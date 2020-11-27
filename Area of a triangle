from tkinter import *

def main(p1x,p1y,p2x,p2y,p3x,p3y):

    class Point:
        def __init__(self,X,Y):
            self.X = X
            self.Y = Y
            self.Y = Y

    p1 = Point(p1x,p1y)
    p2 = Point(p2x,p2y)
    p3 = Point(p3x,p3y)

    def hypo(x1,x2,y1,y2):
        a = (((x1 - x2)**2)**0.5)
        b = (((y1 - y2)**2)**0.5)
        c = ((a**2)+(b**2))**0.5

        return(c)

    def area(a,b,c):
        return(0.25 * (((a+b+c)*(-a+b+c)*(a-b+c)*(a+b-c))**0.5))


    lens = []

    lens.append(hypo(p1.X,p2.X,p1.Y,p2.Y))
    lens.append(hypo(p3.X,p2.X,p3.Y,p2.Y))
    lens.append(hypo(p1.X,p3.X,p1.Y,p3.Y))

    arin = (round(area(lens[0],lens[1],lens[2]),4))

    return(arin)


root = Tk()
root.title("Area Of A Triangle")

greeting = Label(root,text="Enter Three Points of a Triangle",fg="gold",bg="grey")
header1 = Label(root,text="Enter Point 1 Coordinates Below: ")
header2 = Label(root,text="Enter Point 2 Coordinates Below: ")
header3 = Label(root,text="Enter Point 3 Coordinates Below: ")


field1 = Entry(root,width=20,bg="gold")
field2 = Entry(root,width=20,bg="gold")
field3 = Entry(root,width=20,bg="gold")
field4 = Entry(root,width=20,bg="gold")
field5 = Entry(root,width=20,bg="gold")
field6 = Entry(root,width=20,bg="gold")

xlabel1 = Label(root,text="X:")
xlabel2 = Label(root,text="X:")
xlabel3 = Label(root,text="X:")
ylabel1 = Label(root,text="Y:")
ylabel2 = Label(root,text="Y:")
ylabel3 = Label(root,text="Y:")

def click():
    p1x=int(field1.get())
    p1y=int(field2.get())
    p2x=int(field3.get())
    p2y=int(field4.get())
    p3x=int(field5.get())
    p3y=int(field6.get())


    area = main(p1x,p1x,p2x,p2y,p3x,p3y)


    label = Label(root,text=(str(area)))
    label.grid(row=8,column=1)


button = Button(root,text="Get Area!",command=click,fg="gold",bg="grey")


greeting.grid(row=0,column=1)

header1.grid(row= 1, column= 1)

xlabel1.grid(row=2,column=0)
ylabel1.grid(row=2,column=2)
field1.grid(row= 2, column= 1)
field2.grid(row= 2, column= 3)

header2.grid(row= 3, column= 1)

xlabel2.grid(row=4,column=0)
ylabel2.grid(row=4,column=2)
field3.grid(row= 4, column= 1)
field4.grid(row= 4, column= 3)

header3.grid(row= 5, column= 1)

xlabel3.grid(row=6,column=0)
ylabel3.grid(row=6,column=2)
field5.grid(row= 6, column= 1)
field6.grid(row= 6, column= 3)

button.grid(row=7,column=1)

root.mainloop()



