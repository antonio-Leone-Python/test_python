# test_python

#EREDITARIETA': capacità di ereditare da una o piu classi "padre" attribbuti o metodi

class Calcolo:
    def __init__(self,a,b):       
        self.a=a
        self.b=b

    def usa_calcolo(self):
        c=self.a+self.b
        print(c)


class Addizione(Calcolo):# LA CLASSE ADDDZIONE EREDITA METODI E ATTRIBUTI DA CALCOLO
    def __init__(self,a,b):
        super().__init__(a,b)

addizione=Addizione(4,5)
addizione.usa_calcolo()   

#POLIMORFISMO: capacità del codice dicambiare composrtamento ma non forma
class Cane:             #creiamo la classe cane con metodo "suona"
    def suona(self):
        print("abbaia")

class Gatto:          #ora creiamo un altra classe con il nome "gatto" con lo stesso metodo di prima
    def suona(self):
        print("miagola")  



cane = Cane()
gatto = Gatto()
gatto.suona()
cane.suona()


#INCAPSULAMENTO  #INCAPSULAMENTO     L' INCAPSULAMENTO E' LA CAPACITA' DEL CODICE DI NASCONDERE DATI ANCHE A SE STESSO
# POSSIAMO TROVARE "__" CHE STA A SIFGNIFICARE CHE QUEL DATO E' PRIVATO O "_" CHE STA A SIGNIFICARE CHE QUEL DATO E' PROTETTO
class Persona:
    def __init__(self, nome, cognome):
        self.__nome = nome
        self.__cognome = cognome

    def get_nome(self):
        return self.__nome

    def set_nome(self, nome):
        self.__nome = nome

    def get_cognome(self):
        return self.__cognome

    def set_cognome(self, cognome):
        self.__cognome = cognome

#INCAPSULAMENTO     L' INCAPSULAMENTO E' LA CAPACITA' DEL CODICE DI NASCONDERE DATI ANCHE A SE STESSO
# POSSIAMO TROVARE "__" CHE STA A SIFGNIFICARE CHE QUEL DATO E' PRIVATO O "_" CHE STA A SIGNIFICARE CHE QUEL DATO E' PROTETTO

class Persona:
    def __init__(self, nome, cognome):
        self.__nome = nome
        self.__cognome = cognome

    def get_nome(self):
        return self.__nome

    def set_nome(self, nome):
        self.__nome = nome

    def get_cognome(self):
        return self.__cognome

    def set_cognome(self, cognome):
        self.__cognome = cognome


persona=Persona("mirko","campari")
print(persona.get_nome())
print(persona.get_cognome())
      


        







