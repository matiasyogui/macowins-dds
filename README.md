# macowins-dds
# Ejercicio diagnostico de Diseño de sistemas #
## Matias Ezequiel Yogui Arakaki ##

### Enunciado: ### https://docs.google.com/document/d/1mjWKl9YH9Bb39iIUl1bQj_xhx_-CjCAMpcAXRqKhVjU/edit

### Requerimientos: ###
1. Saber precio de venta:
    * Nueva: no se modifica el precio base.
    * Promoción: se resta un valor fijo decidido por el usuario.
    * Liquidación: 50% del valor del producto.
2. Saber tipos de prenda (sacos, pantalones o camisas)
3. Registrar las ventas y saber las ganancias de un determinado día.
    * Cada venta tiene las prendas, cantidad y fecha de venta.
    * Pueden ser en efectivo (no se modifica el precio) o con tarjeta (recargo según la cantidad de cuotas seleccionadas. Cantidad de cuotas * coeficiente fijo + 0.01 del valor de cada prenda)

### Diagrama de clases: ###
![](https://github.com/matiasyogui/macowins-dds/blob/main/Diagrama%20de%20clases%20Macowins%20(2).png)

### Aclaraciones: ###
* Para calcular el precio de las prendas, opte por usar composición ya que el estado puede cambiar en el tiempo.
* Para modelar las ventas, senti que era mejor usar una clase abstracta (Venta) aunque me deje una clase vacia (VentaEfectivo).
