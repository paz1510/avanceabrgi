mport math




def MenuPrincipal():
  print("\n======Calculadora para carpinteria y diseño de interiores======")
  print("1. Calcular Área")
  print("2. Calcular Perímetro")
  print("3. Calcular Volumen")
  print("4. Salir")




def SubmenuArea():
  print("\n=====Cálculo Área======")
  print("1. Forma Cuadrada")
  print("2. Forma Rectángular")
  print("3. Forma Círcular")
  print("4. Volver")




def SubmenuPerimetro():
  print("\n======Calculo Perímetro======")
  print("1. Forma Cuadrada")
  print("2. Forma Rectángular")
  print("3. Forma Círcular")
  print("4. Volver")
def SubmenuVolumen():
  print("\n======Volumen =======")
  print("1. Cubo")
  print("2. Prisma Rectangular")
  print("3. Cilindro")
  print("4. Volver")




while True:
  MenuPrincipal()
  Opcion = input("Elige una opción: ")




  if Opcion == "1":
      while True:
          SubmenuArea()
          Forma = input("Elige una forma: ")




          if Forma == "1":
              Lado = float(input("Ingrese Medida Lado del cuadrado: "))
              AreaCuadrado =Lado * Lado
              print("El Área es:", AreaCuadrado)
          if Forma == "2":
              Base = float(input(" Ingrese Medida Base: "))
              Altura = float(input("Ingrese Medida Altura: "))
              AreaRectangulo = Base * Altura
              print("El Área es:", AreaRectangulo)
          if Forma == "3":
              Radio = float(input(" Ingrese Medida Radio: "))
              AreaCirculo = math.pi * Radio * Radio
              print("El Área es:", AreaCirculo)
          if Forma == "4":
              break




  if Opcion == "2":
      while True:
          SubmenuPerimetro()
          Forma = input("Elige una forma: ")




          if Forma == "1":
              Lado = float(input("Ingrese Medida Lado del cuadrado: "))
              PerimetroCuadrado = 4 * Lado
              print("El Perímetro es:",PerimetroCuadrado)
          if Forma == "2":
              Base = float(input("Base: "))
              Altura = float(input("Altura: "))
              PerimetroRectangulo = 2 * (Base + Altura)
              print("El Perímetro es:", PerimetroRectangulo)
          if Forma == "3":
              Radio = float(input("Radio: "))
              PerimetroCirculo = 2 * math.pi * Radio
              print("El Perímetro es:", PerimetroCirculo)
          if Forma == "4":
              break




  if Opcion == "3":
      while True:
          SubmenuVolumen()
          Forma = input("Elige una forma: ")




          if Forma == "1":
              Lado = float(input("Ingrese Medida de Lado del cubo: "))
              VolumenCubo = Lado ** 3
              print("Volumen:", VolumenCubo )
          if Forma == "2":
              Largo = float(input("Ingrese Medida del Largo: "))
              Ancho = float(input("Ingrese Medida del Ancho: "))
              Alto = float(input("Ingrese Medida del Alto: "))
              VolumenPrimaRectangular = Largo * Ancho * Alto
              print("El Volumen es:",VolumenPrimaRectangular )
          if Forma == "3":
              Radio = float(input("Ingrese Medida del Radio: "))
              Altura = float(input("Ingrese Medida de la Altura: "))
              VolumenCilindro = math.pi * Radio * Radio * Altura
              print("El Volumen es:", VolumenCubo)
          if Forma == "4":
              break




  if Opcion == "4":
      print("Gracias por usar la calculadora para carpinteria y diseño de interiores.")
      break
