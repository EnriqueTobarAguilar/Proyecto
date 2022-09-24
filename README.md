# Proyecto Final Algoritmos y Programación
Ahorcado de Universidades de Colombia

Proyecto Realizado por: Jaime Enrique Tobar Aguilar estudiante de Ingenieria de Producción de la Universidad Ean📚👌😏


Introducción 


Proyecto de la unidad de estudio de algoritmos y programación impartida por el profesor Brayan torres de la universidad ean para los estudiantes de la universidad ean con el objetivo de dar bases para solucionar problemas, es por esto que el objetivo es aplicar lo aprendido en clase he desarrollado un código en replit con Python con diferentes nombres de universidades de Colombia.



A continuación encontrara el proceso de cómo se desarrolló el código de Python para jugar ahorcado en la consola de Python online para disfrutar de este juego básico:

Para iniciar podemos importar el módulo Random que funciona como generador pseudoaleatorios para varias distribuciones en la secuencia eligiendo de manera aleatoria los datos.


Después se dan condiciones con for, while, if definiendo todos los parámetros para que al ejecutar el programa este escoja una de las universidades para así ingresar palabra a palabra hasta completar la palabra. El codigo break se usa para cerrar el bucle generalmente despues de un if.



Con esto se logra culminar este proyecto que para mí como ingeniero me genera esa habilidad para pensar y solucionar problemas de alta complejidad gracias a la exigencia durante lo visto en la unidad de estudió.

#JUEGO de Entretenimiento comunmente llamado ahorcado
import random

def palabra()->str:

  palabras=["universidad", "andes", "rosario","pedagogica","javeriana","santo tomas","andina","catolica","sabana", "militar","santander","antioquia","nacional","bosque"]
  
  numero=random.randint(0, len(palabras)-1)
  
  
  return palabras[numero]
  
a=palabra()

b=[]

for i in range(0,len(a)):

  b.append("_")
  
print(a)

while True:

  letra=str(input("Digite letra: "))
  
  for x in range(0,len(a)):
  
    if(a[x]==letra):
    
      b[x]=letra  
      
  print("".join(b))  
  
  x="".join(b)
  
  if(x==a):
  
    print("Ganaste(●'◡'●)")
    
    break
    
