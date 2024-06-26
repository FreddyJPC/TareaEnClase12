import org.junit.Assert.* 

fun main() {

 esMayorDeEdad_personaMayorDeEdad_devuelveTrue()
 esMayorDeEdad_personaMenorDeEdad_devuelveFalse()
 esMayorDeEdad_personaLimite_devuelveTrue()
 println("Todos los tests pasaron!")
}

fun esMayorDeEdad(edad: Int): Boolean {
 return if (edad >= 18) {
  true
 } else {
  false
 }
}

fun esMayorDeEdad_personaMayorDeEdad_devuelveTrue() {
 val edad = 20
 val resultado = esMayorDeEdad(edad)
 assertTrue(resultado)
}


fun esMayorDeEdad_personaMenorDeEdad_devuelveFalse() {
 val edad = 17
 val resultado = esMayorDeEdad(edad)
 assertFalse(resultado)
}


fun esMayorDeEdad_personaLimite_devuelveTrue() {
 val edad = 18
 val resultado = esMayorDeEdad(edad)
 assertTrue(resultado)
}
