# factorial-
 ¿que es la funcion factorial?

 Una función es un bloque de código que realiza alguna operación. Una función puede definir opcionalmente parámetros de entrada que permiten a los llamadores pasar argumentos a la función. Una función también puede devolver un valor como salida.

 # Ejemplos de fórmulas factoriales

1! = 1 * 1 = 1
3! = 1 * 2 * 3 = 6
10! = 1 * 2 * 3 … 8 * 9 * 10 = 3.628.800

Qué pasa con el 0 factorial, ¿cómo calcularlo? Si volvemos a la definición de función factorial podemos ver que no tiene sentido aplicarla en el caso del “0”. No existen números positivos anteriores al 0 por lo que 0 x 0 = 0.

No obstante, se ha acordado que en el caso de 0 factorial el resultado será igual a 1:

0! = 0 x 0 = 1

# En Kotlin, puedes implementar la función factorial de manera similar a otros lenguajes, utilizando recursión o iteración. Aquí te muestro ambos enfoques en Kotlin:

fun factorial(n: Int): Long {
    return if (n == 0) {
        1
    } else {
        n * factorial(n - 1)
    }
}

fun main() {
    println(factorial(5))  // Salida: 120
}



fun factorial(n: Int): Long {
    var result = 1L
    for (i in 1..n) {
        result *= i
    }
    return result
}

fun main() {
    println(factorial(5))  // Salida: 120
}


 
