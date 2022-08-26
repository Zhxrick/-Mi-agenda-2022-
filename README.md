
### Programacion general 

Sub sena

nom = "Luis"
num = "10"
nom = "Maria"

end Sena

### FECHA: 19/08/2022

Sub Suma()
 a = Int(InputBox("digitar numero para la variable a"))
 b = Int(InputBox("Digitar numero para la variable b"))
 
 c = a + b
 
 MsgBox "El resultado es:" & c


End Sub


### Descuento numero de noche

definir noche, precio, pago como entero
	definir descuento como real
	
	precio<- 100
	escribir "Digite el numero de noches"
	leer noches
	
	total <- precio * noches
	
	si noches > 3 entonces 
		descuento <- total*.05
		
		 escribir "Su pago total es: ", total - descuento 
	sino 
		
		escribir "su pago total sin descuento es: ", total
		
		
	FinSi

### Sacar promedio de notas / aprobado no aprobado 
Algoritmo sin_titulo
	
	definir alumno como caracter 
	definir examenparcial, examenfinal,promediopracticas como real
	definir final Como Real
	
	escribir "Digite el nombre del alumno" 
	leer alumno 
	
	Escribir "Las notas se calificaran de 1 - 10" 
	
	Escribir "Digite la nota del examen parcial"
	leer examenparcial
	Escribir "Digite la nota del examen final"
	leer examenfinal
	Escribir "Digite la nota del promedio de practicas"
	leer promediopracticas
	
	final <- (examenparcial+promediopracticas+(examenfinal*2))/3
	
	si final > 6 entonces 
		escribir "alumno aprobado: ", alumno 
		escribir "su promedio es: ", final 
	sino 
		
		escribir alumno, " alumno no aprobado"
		escribir "su promedio es: ", final 
		
	FinSi
	
FinAlgoritmo

	
	
	
	



