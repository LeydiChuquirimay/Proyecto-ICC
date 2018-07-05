# Proyecto-ICC
opcion=-1
preferencia=-1
def menu():
    print()
    print("************************************************************")
    print("menu de opciones:")
    print("1. Ingresar datos:")
    print("2. Recomendación de Ejercicios:")
    print("3. Eleccion de Ejercicios:")
    print("el programa finaliza si ingresa el valor 0.")
    print("************************************************************")
    print()

def Ejercicios():
    print("1. Corrige tu postura")
    print("2. Regula tu peso")
    print("3. Zonas complicadas")
    print("4. Recupera tu energia")
    print("5. Tonifica tu cuerpo")

#Rutinas segun imc :
bajopeso = ["estiramiento","press de banca","sentadillas","press de hombros","Haye tgp", ]
pesonormal = ["estiramiento","explosion de burpes","squat jumps","jumping lunges","jumpick jacks"]
sobrepeso = ["estiramiento","rotacion de troncos","cardio","Overhead squat","Lunge","Sumo Deadlift","Sit up",]
obesidad = ["estiramiento","juck jumps","Knee up"," cardio"]
# segun las lista de ejercicios  :
postura = ["pesas","face pulls","plank","sentadilla globel"]
zonascom = ["bicicletas","saltar cuerda","abdomianles"]
tonificacion = ["Sentadillas con mancuernas","Zancadas con mancuernas","Puente de glúteo","plancha abdominales" ]

ejercicios=[]

print("********Bienvenidos********")
menu()

while opcion != 0:
    opcion = int(input("ingrese la opción de operación:"))

    if opcion == 1:
        print("Ingrese su talla:")
        Talla = float(input())
        print("ingrese su peso:")
        Peso = float(input())
        print("Ingrese su edad:")
        Edad = float(input())
        T= Talla**2
        Imc= round(Peso/T)
        print("Su Indice de masa corporal es:")
        print(Imc)
        menu()
    elif opcion == 2:
        print("Usted tiene:")
        if Imc < 18.5:
            x = "bajo peso"
            print(x)
            print("Le recomendamos esta rutina:")
            print(bajopeso)
        elif 18.5<=Imc<=24.9:
            x = "peso normal"
            print(x)
            print("Elija que rutina quiere hacer en la opcion 3")

        elif Imc>=25.0:
            x = "sobre peso"
            print(x)
            print("Le recomendamos esta rutina:")
            print(sobrepeso)
        elif 25.0<=Imc<=29.9:
            x = "preobesidad"
            print(x)
            print("Le recomendamos estas rutinas:")
            print(sobrepeso)
            print(obesidad)
        elif 30<=Imc:
            x = "obesidad"
            print(x)
            print("Le recomendamos esta rutina:")
            print(obesidad)
        menu()
    elif opcion == 3:
        Ejercicios()
        preferencia = int(input("ingrese la opción de preferencia:"))

        while preferencia!=0:
            if preferencia == 1:
                y=0
                print(postura)
            elif preferencia == 2:
                y=0
                print()
            elif preferencia == 3:
                y=0
                print(zonascom)
            elif preferencia == 4:
                y=0
                print(zonascom)
            elif preferencia == 5:
                y=0
                print(tonificacion)
        menu()

    elif opcion == 0:
        print("gracias por utilizar el software.")
