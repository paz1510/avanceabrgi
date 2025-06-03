import math
import LIBRERIA.Validaciones as Valid
import LIBRERIA.OperacionesMatematicas as Calculadora

ContadorCuadrados = 0
ContadorRectangulos = 0
ContadorCirculos = 0
ContadorCubos = 0
ContadorPrismas = 0
ContadorCilindros = 0

def MenuPrincipal():
    print("\n====== Calculadora para carpintería y diseño de interiores ======")
    print("\n====== MENÚ PRINCIPAL======")
    print("1. Calcular Área")
    print("2. Calcular Perímetro")
    print("3. Calcular Volumen")
    print("4. Salir y Mostrar reporte")

def SubmenuArea():
    print("\n===== Cálculo Área ======")
    print("\n====== SubMenuArea======")
    print("1. Forma Cuadrada")
    print("2. Forma Rectangular")
    print("3. Forma Circular")
    print("4. Volver")

def SubmenuPerimetro():
    print("\n====== Cálculo Perímetro ======")
    print("\n====== SubMenuPerímetro======")
    print("1. Forma Cuadrada")
    print("2. Forma Rectangular")
    print("3. Forma Circular")
    print("4. Volver")

def SubmenuVolumen():
    print("\n====== Cálculo Volumen =======")
    print("\n====== SubMenuVolunen======")
    print("1. Cubo")
    print("2. Prisma Rectangular")
    print("3. Cilindro")
    print("4. Volver")

while True:
    MenuPrincipal()
    Opcion = input("Elige una opción:\t\t\t")

    if Opcion == "1":
        while True:
            SubmenuArea()
            Forma = input("Elige una forma:\t\t\t")

            if Forma == "1":
                while True:
                    Lado = float(input("Ingrese Medida Lado del cuadrado (METROS):\t\t\t"))
                    if Valid.ValidarMedida(Lado):
                        break
                AreaCuadrado = Calculadora.AreaCuadrado(Lado)
                print("\n===== RESULTADOS =====")
                print("Medida de lado ingresado:", Lado)
                print("El Área es:", AreaCuadrado, "m²")
                ContadorCuadrados += 1

            elif Forma == "2":
                while True:
                    Base = float(input("Ingrese Medida Base (METROS):\t\t\t"))
                    if Valid.ValidarMedida(Base):
                        break
                while True:
                    Altura = float(input("Ingrese Medida Altura (METROS):\t\t\t"))
                    if Valid.ValidarMedida(Altura):
                        break
                AreaRectangulo = Calculadora.AreaRectangulo(Base, Altura)
                print("\n===== RESULTADOS =====")
                print("Medida de Base ingresado:", Base)
                print("Medida de Altura ingresado:", Altura)
                print("El Área es:", AreaRectangulo, "m²")
                ContadorRectangulos += 1

            elif Forma == "3":
                while True:
                    Radio = float(input("Ingrese Medida Radio (METROS):\t\t\t"))
                    if Valid.ValidarMedida(Radio):
                        break
                AreaCirculo = Calculadora.AreaCirculo(Radio)
                print("\n===== RESULTADOS =====")
                print("Medida de Radio ingresado:", Radio)
                print("El Área es:", AreaCirculo, "m²")
                ContadorCirculos += 1

            elif Forma == "4":
                break
            else:
                print("ERROR: Opción no válida. Intente nuevamente e Ingrese 1 o 2 o 3 o 4.")

    elif Opcion == "2":
        while True:
            SubmenuPerimetro()
            Forma = input("Elige una forma: ")

            if Forma == "1":
                while True:
                    Lado = float(input("Ingrese Medida Lado del cuadrado (METROS):\t\t\t"))
                    if Valid.ValidarMedida(Lado):
                        break
                PerimetroCuadrado = Calculadora.PerimetroCuadrado(Lado)
                print("\n===== RESULTADOS =====")
                print("Medida de lado ingresado:", Lado)
                print("El Perímetro es:", PerimetroCuadrado, "m")
                ContadorCuadrados += 1

            elif Forma == "2":
                while True:
                    Base = float(input("Ingrese Medida Base (METROS):\t\t\t"))
                    if Valid.ValidarMedida(Base):
                        break
                while True:
                    Altura = float(input("Ingrese Medida Altura (METROS):\t\t\t"))
                    if Valid.ValidarMedida(Altura):
                        break
                PerimetroRectangulo = Calculadora.PerimetroRectangulo(Base, Altura)
                print("\n===== RESULTADOS =====")
                print("Medida de Base ingresado:", Base)
                print("Medida de lado ingresado:", Altura)
                print("El Perímetro es:", PerimetroRectangulo, "m")
                ContadorRectangulos += 1

            elif Forma == "3":
                while True:
                    Radio = float(input("Ingrese Medida Radio (METROS):\t\t\t"))
                    if Valid.ValidarMedida(Radio):
                        break
                PerimetroCirculo = Calculadora.PerimetroCirculo(Radio)
                print("\n===== RESULTADOS =====")
                print("Medida de Radio ingresado:", Radio)
                print("El Perímetro es:", PerimetroCirculo, "m")
                ContadorCirculos += 1

            elif Forma == "4":
                break
            else:
                print("ERROR: Opción no válida. Intente nuevamente e Ingrese 1 o 2 o 3 o 4.")

    elif Opcion == "3":
        while True:
            SubmenuVolumen()
            Forma = input("Elige una forma:\t\t\t")

            if Forma == "1":
                while True:
                    Lado = float(input("Ingrese Medida de Lado del cubo(METROS):\t\t\t"))
                    if Valid.ValidarMedida(Lado):
                        break
                VolumenCubo = Calculadora.VolumenCubo(Lado)
                print("\n===== RESULTADOS =====")
                print("Medida de lado ingresado:", Lado)
                print("El Volumen es:", VolumenCubo, "m³")
                ContadorCubos += 1

            elif Forma == "2":
                while True:
                    Largo = float(input("Ingrese Largo (METROS):\t\t\t"))
                    if Valid.ValidarMedida(Largo):
                        break
                while True:
                    Ancho = float(input("Ingrese Ancho (METROS):\t\t\t"))
                    if Valid.ValidarMedida(Ancho):
                        break
                while True:
                    Alto = float(input("Ingrese Alto (METROS):\t\t\t"))
                    if Valid.ValidarMedida(Alto):
                        break
                VolumenPrisma = Calculadora.VolumenPrisma(Largo, Ancho, Alto)
                print("\n===== RESULTADOS =====")
                print("Medida de Largo ingresado:", Largo)
                print("Medida de Ancho ingresado:", Ancho)
                print("Medida de Alto ingresado:", Alto)
                print("El Volumen es:", VolumenPrisma, "m³")
                ContadorPrismas += 1

            elif Forma == "3":
                while True:
                    Radio = float(input("Ingrese Radio (METROS):\t\t\t"))
                    if Valid.ValidarMedida(Radio):
                        break
                while True:
                    Altura = float(input("Ingrese Altura (METROS):\t\t\t"))
                    if Valid.ValidarMedida(Altura):
                        break
                VolumenCilindro = Calculadora.VolumenCilindro(Radio, Altura)
                print("\n===== RESULTADOS =====")
                print("Medida de Radio ingresado:", Radio)
                print("Medida de Altura ingresado:", Altura)
                print("El Volumen es:", VolumenCilindro, "m³")
                ContadorCilindros += 1

            elif Forma == "4":
                break
            else:
                print("ERROR: Opción no válida. Intente nuevamente e Ingrese 1 o 2 o 3 o 4.")

    elif Opcion == "4":
        print("\n====== Gracias por usar la calculadora para carpintería y diseño de interiores. ======")
        print("\n===== Estadísticas Utilizadas de Cantidad de Cálculos por Forma =====")
        print("Cantidad de Cálculos de Cuadrados utilizados:", ContadorCuadrados)
        print("Cantidad de Cálculos de Rectángulos utilizados:", ContadorRectangulos)
        print("Cantidad de Cálculos de Círculos utilizados:", ContadorCirculos)
        print("Cantidad de Cálculos de Cubos utilizados:", ContadorCubos)
        print("Cantidad de Cálculos de Prismas rectangulares utilizados:", ContadorPrismas)
        print("Cantidad de Cálculos de Cilindros utilizados:", ContadorCilindros)
        break

    else:
        print("ERROR: Opción no válida. Intente nuevamente e Ingrese 1 o 2 o 3 o 4.")
