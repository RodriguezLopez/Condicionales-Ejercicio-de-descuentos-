# Caso
# Imagina que la tienda donde usted trabaja ofrece descuentos a los clientes en navidad, de acuerdo con el monto de su compra.
# El criterio para establecer el descuento se muestra a continuación:
# Compra (USD)
# Porcentaje
# Si es menor a 80
# 0%
# Si es mayor o igual a 80 y menor que 150
# 10%
# Si es mayor o igual a 150 y menor o igual a 300 
# 15%
# Si es mayor a 300 y menor a 500 
# 20%
# Teniendo en cuenta la tabla, te piden que escribas un programa que solicite el 
# nombre del cliente y el valor de la compra. Y que arroje como resultado: 
# Nombre del cliente
# Valor de la compra sin descuento
# Valor de la compra con descuento.
# Recuerde que para calcular el descuento primero debe multiplicar el valor de la compra por el porcentaje. Luego, 
# debe restar el valor obtenido al valor de la compra y con eso obtiene el precio con descuento.
# descuento = valor_compra x porcentaje
# precio final = valor_compra - descuento

nombre = input("Ingrese su nombre: ")
valor_compra = float(input("Ingrese su valor de compra: "))


if valor_compra < 80:
    print(f"Holas,{nombre}. El valor a pagar es:${valor_compra}")
    
elif valor_compra  >= 80 and valor_compra  < 150:
        descuento = 0.10
        preciofinal = valor_compra -(valor_compra * descuento) 
        print(f"Hola, {nombre}. Tienes un descueto de 10% ")
        print(f"Valor original sin descuento es de {valor_compra:.2f}")
        print(f"El valor con descuento es de {preciofinal:.2f}")
        
elif  valor_compra >= 150 and  valor_compra <= 300:
        descuento = 0.15
        preciofinal = valor_compra -(valor_compra * descuento) 
        print(f"Hola, {nombre}. Tienes un descueto de 15% ")
        print(f"Valor original sin descuento es de $: {valor_compra:.2f}")
        print(f"El valor con descuento es de $: {preciofinal:.2f}")
            
elif valor_compra > 300 and valor_compra <500:
        descuento = 0.20
        preciofinal = valor_compra -(valor_compra * descuento) 
        print(f"Hola, {nombre}. Tienes un descueto de 20% ")
        print(f"Valor original sin descuento es de {valor_compra:.2f}")
        print(f"El valor con descuento es de {preciofinal:.2f}")
else:
    print(f"Hola{nombre}. Compra mayor 500, consulta descuentos especiales en tienda")
            
    
