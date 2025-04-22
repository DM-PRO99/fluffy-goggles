#ejercicio compra de Productos
#Datos de Entrada

nombrecliente= ""
while nombrecliente == "":
    print("Ingresa Tu Nombre:")
    nombrecliente = input()
    
nombreproducto = ""
while nombreproducto == "":
    print("Ingresa el nombre del Producto:")
    nombreproducto = input()
    
PrecioUNitario=float (input("Valor unitario del producto:"))
while PrecioUNitario < 1:
    print("Ingresa un valor mayor a o pesos")
    PrecioUNitario=float(input())

Cantidad=int(input("Ingrese la cantidad:"))
while Cantidad< 1:
    print("ingresa una cantidad mayor a o")
    Cantidad=float(input())

PorcentajeDescuento=float(input("Ingrese el descuento:(Descuento del 10%): "))

while PorcentajeDescuento <1:
    print("ingresa un descuento superior a 1%")
    PorcentajeDescuento=float(input())

#procesamiento 
#calcular el precio total sin el descuent#o
preciototal= PrecioUNitario*Cantidad

#calcular el monto del descuento
descuento=float(PorcentajeDescuento/100)*preciototal

#calcular el precio final despues del descuento
preciofinal=preciototal-descuento

#mostar resultados
print(f"Hola: {nombrecliente}")
print(f"Resumen de la compra:")
print(F"producto:{nombreproducto}")
print(f"Hola:{nombrecliente} el valor del producto Unitario es:${PrecioUNitario:.2f}")
print(f"Cantidad:{Cantidad}")
print(f"Precio Total:{nombrecliente} sin descuento es:${preciototal:.2f}")
print(f"El Ahorro es: ${descuento:.2f}")
print(f"EL Precio final a pagar por tu:{nombreproducto} es:${preciofinal:.2f}")

print(f"Gracias por tu compra {nombrecliente} pronto regreso")
