# calculadora_descuento
Este programa en Python solicita al usuario el precio de un producto y el porcentaje de descuento, calcula el monto final a pagar y lo muestra en pantalla.

def aplicar_descuento(precio, porcentaje):
 
    descuento = precio * (porcentaje / 100)
    precio_final = precio - descuento
    return precio_final


def calcular_descuento():
   
    precio_original = float(input("Ingrese el precio original del producto: "))
    porcentaje_descuento = float(input("Ingrese el porcentaje de descuento: "))
    precio_final = aplicar_descuento(precio_original, porcentaje_descuento)
    def mostrar_resultado(monto_final):
        print(f"\nEl monto final a pagar después del descuento es: ₡{monto_final:.2f}")
    mostrar_resultado(precio_final)


calcular_descuento()
