# Documentacion Del Proyecto
 Juego simple adivina el numero

import random
Importa la librería random.
Sirve para generar números aleatorios.


numero_secreto = random.randint(1, 10)
Genera un número aleatorio entre 1 y 10.
Ese número se guarda en la variable numero_secreto.

Ejemplo:

numero_secreto = 7
intentos = 3
Define que el jugador tendrá 3 intentos para adivinar.


print(" Bienvenido al juego")
print("Adivina el número entre 1 y 10")
Muestra mensajes de bienvenida en pantalla.


while intentos > 0:
Crea un ciclo que se repetirá mientras queden intentos.


intento = int(input("Ingresa un número: "))
Pide al usuario escribir un número.
input() recibe texto.
int() convierte ese texto en número entero.


if intento == numero_secreto:
Compara el número ingresado con el número secreto.


Si son iguales:

print(" ¡Correcto! Ganaste")
break
Muestra mensaje de victoria.
break termina el ciclo inmediatamente.



Si el número es incorrecto:

else:
    intentos -= 1
Resta 1 intento.

Ejemplo:

3 → 2 → 1 → 0
print(" Incorrecto")
Muestra que el usuario falló.
if intentos > 0:
Verifica si todavía quedan intentos.

Si quedan:

print(f"Te quedan {intentos} intentos")
Muestra cuántos intentos faltan.

Si ya no quedan:

print(f" Perdiste. El número era {numero_secreto}")
Muestra mensaje de derrota.
Revela el número secreto.