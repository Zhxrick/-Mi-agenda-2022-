
### Programacion general 
´´´´


Sub sena

nom = "julissa" 
num = "10" 
nom = "zharick" 

end Sena

´´´´
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


### Impuesto anual de una empresa usando If - Else

Sub sena()

    ingreso_anual = InputBox("Digite los ingresos anuales de la empresa: ")
    Total = 0
    impuesto = 0
    aumento = 0
    
    If ingreso_anual < 1000 And ingreso_anual > 0 Then
      MsgBox ("No debe pagar impuestos")
    Else
        If ingreso_anual >= 1001 And ingreso_anual <= 10000 Then
            aumento = (ingreso_anual * 0.05)
            MsgBox ("Total impuesto a pagar: ") & aumento
        Else
            If ingreso_anual >= 10001 And ingreso_anual <= 100000 Then
            aumento = (ingreso_anual * 0.1)
            MsgBox ("Total impuesto a pagar: ") & aumento
            
            Else
                If ingreso_anual >= 100001 And ingreso_anual <= 1000000 Then
                    aumento = (ingreso_anual * 0.15)
                    MsgBox ("Total impuesto a pagar: ") & aumento
                Else
                      If ingreso_anual >= 100000 And ingreso_anual <= 10000000 Then
                         aumento = (ingreso_anual * 0.2)
                          MsgBox ("Total impuesto a pagar: ") & aumento
                      Else
                           If ingreso_anual >= 10000001 Then
                                aumento = (ingreso_anual * 0.25)
                                MsgBox ("Total impuesto a pagar: ") & aumento
                            Else
                                MsgBox "No se puede calcular"
                           End If
                          
                      End If
                
                End If
                
            End If
                    
        End If

    End If

End Sub
 
 ### Impuesto anual de una empresa usando Case 
 
 Sub sena()

      ingreso_anual = Int(InputBox("Digite los ingresos anuales de la empresa: "))
      aumento = 0
      
      Select Case ingreso_anual
      
      Case 0 To 1000
      MsgBox ("No debe pagar impuestos")
      
      Case 1001 To 10000
      aumento = (ingreso_anual * 0.05)
      MsgBox ("El total de impuestos a pagar es: ") & aumento
      
      Case 10001 To 100000
      aumento = (ingreso_anual * 0.1)
      MsgBox ("El total de impuesto a pagar es: ") & aumento
      
      Case 100001 To 1000000
      aumento = (ingreso_anual * 0.15)
      MsgBox ("El total de impuestos a pagar es: ") & aumento
      
      Case 1000000 To 10000001
      aumento = (ingreso_anual * 0.2)
      MsgBox ("El total de impuestos a pagar es: ") & aumento
      
      End Select
      
      If ingreso_anual >= 10000001 Then
                            aumento = (ingreso_anual * 0.25)
                            MsgBox ("Total impuesto a pagar: ") & aumento
                            
      End If

End Sub

	


### Celdas 


	Sub guardar()
    fila = datos.Cells(2, 7)
    datos.Cells(fila, 1) = formulario.Cells(8, 4)
    datos.Cells(fila, 2) = formulario.Cells(10, 4)
    datos.Cells(fila, 3) = formulario.Cells(12, 4)
    datos.Cells(fila, 4) = formulario.Cells(14, 4)
    MsgBox "Datos guardados"
    datos.Cells(2, 7) = fila + 1
End Sub


### Registro de nombre en celdas excel
	
Sub sena()
        
        For n = 2 To 16
            nombre = InputBox("Digite su nombre: " & n)
            datos.Cells(n, 1) = nombre
        
            
        Next n
        

End Sub

### Recaudo de fondos 

Sub eventoescolar()
    
	    abono = 0
	    no_abono = 0
	    diezmil = 0
	    recaudado = 0

	    For a = 1 To 2
		situacion = InputBox("Desea abonar para el evento? (si o no)")
		If situacion = "si" Then
		    abono = abono + 1
		    Total = Int(InputBox("Cuanto va a abonar?"))
		    recaudado = recaudado + Total
		    If Total >= 10000 Then
			diezmil = diezmil + 1
		    End If
		Else
		    no_abono = no_abono + 1
		End If
	    Next a

	    promedio = total_recaudado / abono
	    MsgBox "El total recaudado es de $" & recaudado
	    MsgBox "El promedio del recaudo es de $" & promedio
	    MsgBox "La cantidad de estudiantes que donaron " & "(" & abono & ")" & " Estudiantes"
	    MsgBox "La cantidad de estudiantes que no donaron " & "(" & no_abono & ")" & " Estudiantes"
	    MsgBox "Los estudiantes que aportaron una cantidad superior a $10.000:   " & "(" & diezmil & ")" & " Estudiantes"
        
End Sub

### Recaudosb de fondos en PSeint 
                Algoritmo sin_titulo
		
		definir no_abono Como Real
		definir abono Como entero 
		definir abonomasdiezmil como real 
		definir recaudado como real 
		definir promedio como real 
		definir cantidadestudiantes Como Entero
		
		numestudiantes <- 2 
		
		para d<-1 hasta numestudiantes Hacer
			escribir "Desea aportar para la recolecta (si o no)"
			leer estudiante 
			si estudiante = "si" entonces 
				abono <- abono + 1 
				escribir "que cantidad va a aportar?"
				leer total 
				recaudado <- recaudado + total 
				si total > 10000 entonces 
					abonomasdiezmil <- abonomasdiezmil + 1 							
				FinSi
			FinSi		
			si estudiante = "no" entonces 
				no_abono <- no_abono + 1	
			FinSi	
		FinPara
		promedio <- recaudado / abono
		
		escribir "El total de recaudado por los estudiantes es: ", recaudado 
		escribir "El promedio recaudado por estudiante es: ", promedio 
		escribir "El numero de estudiantes que aportaron es: ", abono 
		escribir "El numero de estudiantes que no aportaron es: ", no_abono
		escribir "Los estudiantes que aportaron una cantidad superior a 10,000 fueron: ", abonomasdiezmil
		
                FinAlgoritmo

### Funciones de cadenas de caracteres 

		Sub inicio()
	    For a = 2 To 21
	    nom = Hoja1.Cells(a, 1)
	    ultimo = Len(nom) - 1
	    Hoja1.Cells(a, 2) = Mid(nom, ultimo, 2)

	    Next a
	End Sub


