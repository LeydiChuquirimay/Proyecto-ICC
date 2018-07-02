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
