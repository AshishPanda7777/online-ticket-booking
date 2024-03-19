# online-ticket-booking
def singleton(func):
    L=[]
    def inner(*args,**kwargs):
        if len(L)==0:
            L.append(func())
        return L[0]
    return inner
@singleton
class Crack:
    def __init__(self):
        self.tickets=100
    def book(self):
        ticket=int(input('Enter  the number of tickets :'))
        if(self.tickets>=ticket):
            self.tickets -=ticket
            print('Tickets booked succesfully...')
        else:
            print('Tickets are not available currently !')
@singleton
class Leo:
    def __init__(self):
        self.tickets=100
    def book(self):
        ticket=int(input('Enter  the number of tickets :'))
        if(self.tickets>=ticket):
            self.tickets -=ticket
            print('Tickets booked succesfully...')
        else:
            print('Tickets are not available currently !')
@singleton
class Yodha:
    def __init__(self):
        self.tickets=100
    def book(self):
        ticket=int(input('Enter  the number of tickets :'))
        if(self.tickets>=ticket):
            self.tickets -=ticket
            print('Tickets booked succesfully...')
        else:
            print('Tickets are not available currently !')
@singleton
class Hanuman:
    def __init__(self):
        self.tickets=100
    def book(self):
        ticket=int(input('Enter  the number of tickets :'))
        if(self.tickets>=ticket):
            self.tickets -=ticket
            print('Tickets booked succesfully...')
        else:
            print('Tickets are not available currently !')
@singleton
class Saitan:
    def __init__(self):
        self.tickets=100
    def book(self):
        ticket=int(input('Enter  the number of tickets :'))
        if(self.tickets>=ticket):
            self.tickets -=ticket
            print('Tickets booked succesfully...')
        else:
            print('Tickets are not available currently !')

def pvr():
    print('1.Crack\n2.Leo\n3.Yodha\n4.Hanuman\n5.Saitan')
    movie=int(input('choose any  movie :'))
    if movie==1:
        c1=Crack()
        c1.book()
    elif movie==2:
        l1=Leo()
        l1.book()
    elif movie==3:
        y1=Yodha()
        y1.book()
    elif movie==4:
        h1=Hanuman()
        h1.book()
    elif movie==5:
        s1=Saitan()
        s1.book()
    else:
        print('This movie is not available currently.\nChoose the movie which are available right now. ')

        
while(True):
    print('-----------------------------------')
    pvr()


