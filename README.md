# maquina_de_snack

    saldo = float(input("Ingrese su saldo: "))
    cantidad = 0

    while True:
    print("\n===MAQUINA DE SNACKS===")
    print("Saldo disposinible: Bs", saldo)
    print("1. Papas (Bs 1.50)")
    print("2. Chocolate (Bs 2.00)")
    print("3. Refresco (Bs 2.50)")
    print("4. Salir")
       
       opcion = int(input("Seleccione una opción: "))
    if opcion == 1:
        if saldo >= 1.50:
            saldo -= 1.50
            cantidad += 1
            print("Has comprado Papas")
        else:
            print("Saldo insuficiente")
    elif opcion == 2:
        if saldo >= 2.00:
            saldo -= 2.00
            cantidad += 1
            print("Has comprado Chocolate")
        else:
            print("Saldo insuficiente para comprar Chocolate")
    elif opcion == 3:
        if saldo >= 2.50:
            saldo -= 2.50
            cantidad += 1
            print("Has comprado Refresco")
        else:
            print("Saldo insuficiente para comprar Refresco")
    elif opcion == 4:
        break
    else:
        print("Opción invalida. Por favor seleccione una opción del 1 al 4")
        
print("\nCantidad de productos comprados: ", cantidad)
print("Saldo restante: Bs", saldo)
