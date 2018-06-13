# elmejorproyecto
#productora de elasticos
def Ganancia(a):
    ganancia = (22*a - 14.04*a)
    return ganancia
def Tiempo(a,b,c):
    tiempo = ((400*a)/(30*b))/ c
    return tiempo
def Metros(a):
    metros = 400 * a
    return metros
def Kilos_Hilo(a):
    kilos = a*0.78
    return kilos
def Kilos_Caucho(a):
    kilos = a*0.52
    return kilos
a = int(input("Numero de carretes de 5 ligas que desea elaborar: "))
b = int(input("Numero de tiras por maquina: "))
c = int(input("Numero de máquinas que usará: "))
if b < 1 or b > 48:
    print("Error,el numero de tiras no está dentro de los parámetros [1,48]")
elif c < 1 or c > 3:
    print("Error,el numero de máquinas no está dentro de los parámetros [1,3]")

print()
print("La ganancia será de",Ganancia(a),"soles.")
print("Tomará",Tiempo(a,b,c),"horas.")
print("Se utilizarám",Metros(a),"metros de elástico.")
print("Se utilizarán",Kilos_Hilo(a),"kilos de hilo y",Kilos_Caucho(a),"kilos de caucho.")



def pu():
    if p == "P1":
        return 234
    elif p == "P2":
        return 265
    if p == "P3":
        return 278
    elif p == "P4":
        return 299
    if p == "P5":
        return 334
    elif p == "P6":
        return 365
    else:
        print("Error")
def dsct(new_cantidad,p):
    if new_cantidad >= 1000:
        return new_cantidad*0.78*pu()
    elif new_cantidad >= 100 and new_cantidad < 1000:
        return new_cantidad*0.85*pu()
    elif new_cantidad >= 50 and new_cantidad < 100:
        return new_cantidad * 0.95*pu()
    elif new_cantidad > 0 and new_cantidad < 50:
        return new_cantidad*pu()
def obsequio(clave):
    if clave == "CF1":
        return 50
    elif clave == "CF2":
        return 30
    elif clave == "CF3":
        return 10
    else:
        return 0
print("El precio final es de: ", dsct(new_cantidad, p), " y su obsequio es :", obsequio(clave))
