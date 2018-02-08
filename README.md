from math import pi

class Figura(object):
	__lado = 4

	def area(self):
		pass


class Circulo(Figura): 

	def__init__(self, radio=0):
		self.radio= radio

	def area(self):
		return pi*self.radio*self.radio


class Cuadrado(Figura):

	def area(self):
		return self.lado * self.lado

	def perimetro(self):
		return self.lado*4

if __name__ == '__main__':
    
     Circulo = Figura('area')
     Cuadrado = Figura ('area' , 'perimetro')
       print(Circulo.area())
       print(Cuadrado.area())
       print(Cuadrado.perimetro())
