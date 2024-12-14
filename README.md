# LA-27

FILE NAME: structure.py
from abc import ABC, abstractmethod
class NinjaTurtle(ABC):
    @property
    @abstractmethod
    def alias(self):
        pass
    
class Leonardo(NinjaTurtle):
    def  __init__(self, real_name, alias):
        self.real_name = real_name
        self.__alias = alias
    
    @property
    def alias(self):
        return f"{self.__alias}"

class Michelangelo(NinjaTurtle):
    def  __init__(self, real_name, alias):
        self.real_name = real_name
        self.__alias = alias
    
    @property
    def alias(self):
        return f"{self.__alias}"

class Donatello(NinjaTurtle):
    def  __init__(self, real_name, alias):
        self.real_name = real_name
        self.__alias = alias
    
    @property
    def alias(self):
        return f"{self.__alias}"

class Raphael(NinjaTurtle):
    def  __init__(self, real_name, alias):
        self.real_name = real_name
        self.__alias = alias
    
    @property
    def alias(self):
        return f"{self.__alias}"

if __name__ =="__main__":
    leo = Leonardo("Leonardo", "blue")
    gelo = Michelangelo("Michelangelo", "orange")
    tel = Donatello("Donatello", "violet")
    rap = Raphael("Raphael", "red")

    print(leo.alias)
    print(gelo.alias)
    print(tel.alias)
    print(rap.alias)
