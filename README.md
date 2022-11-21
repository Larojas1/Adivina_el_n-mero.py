import random

def adivina_el_número(x):
  print("*" * 10)
  print("Juego adivina el Número!")
  print("*" * 10)
  print("Tu meta es adivinar el número que ha generado el sistema")

  número_aleatorio = random.randint(1, x)  

  option_user = 0 

  while option_user != número_aleatorio:
      option_user = int(input(f"Adivina un número entre el 1 y {x}: ")) #f-string
  
      if option_user < número_aleatorio:
        print("Intentelo de nuevo, su elección es menor al número generado por el sistema")
      elif option_user > número_aleatorio:
        print("Intentelo de nuevo, su elección es mayor al número generado por el sistema")
      
  print(f"Felicidades! has adivinado el número {número_aleatorio} del sistema!")
  

