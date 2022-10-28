
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
	
### Recaudo de fondos con mientras 

Sub sena()

    abono = 0
    no_abono = 0
     diezk = 0
    Total = 0
    
    While Recaudo <= 3000000
        dinero = Int(InputBox("Cuanto va a abonar?"))
        If dinero > 0 Then
            abono = abono + 1
            Recaudo = Recaudo + dinero
            If dinero >= 10000 Then
                diezk = diezk + 1
            End If
        Else
            no_abono = no_abono + 1
        End If
    Wend
    
    promedio = Recaudo / abono
    MsgBox "El total recaudado es de $" & Recaudo
    MsgBox "El promedio del recaudo es de $" & promedio
    MsgBox "La cantidad de estudiantes que donaron " & "(" & abono & ")" & " Estudiantes"
    MsgBox "La cantidad de estudiantes que no donaron " & "(" & no_abono & ")" & " Estudiantes"
    MsgBox "Los estudiantes que aportaron una cantidad superior a $10.000:   " & "(" & diezk & ")" & " Estudiantes"
        
End Sub

### DartPad 

	void main(){


	  Person person = new Person (nom: "Juan", sex:"Masculino" );

	  person.apellido = " Hernandez";
	  person.edad = 18;


	  print("el nombre es:${person.nombre}");
	  print("el apellido es:${person.apellido}");
	  print("El nombre completo es:${person.nombrecompleto()}");
	  print("El sexo es: ${person.sexo}");
	  print("La edad es ${person.edad}");
	  person.edadMas(12);
	}

	  class Person{
	  String? apellido, nombre, sexo;
	  int? edad; 

	  Person({String? sex, String? nom}){
	     sexo = sex;
	     nombre = nom; 
	    }

	  String nombrecompleto (){
	       String? noc = nombre! + apellido!; 
	       return noc;  
	  }

	  void edadMas(int? sm){
	    int s = edad! + sm!; 
	    print("La edad sumada es: $s");

	  }

	  }
	 
### REINO ANIMAL 

void main(){

	  print ("""
		     EL REINO ANIMAL""");



	  Cocodrilo cocodrilo = new Cocodrilo();
	  cocodrilo.nombre = "Cocodrilo";
	  cocodrilo.alimentacion = "Carnivoro";
	  cocodrilo.nacimiento = "Ovíparos";
	  cocodrilo.habitat = "Mixto";

	  print ("""
	  El nombre del animal es: ${cocodrilo.nombre}
	  su tipo de alimentación es: ${cocodrilo.alimentacion}
	  su tipo de desarrollo embrionario es: ${cocodrilo.nacimiento}
	  El habitat donde se encuentran es: ${cocodrilo.habitat}
	  """);

	  Elefante elefante = new Elefante();
	  elefante.nombre = "Elefante";
	  elefante.alimentacion = "Herviboro";
	  elefante.nacimiento = "Vivíparo";
	  elefante.habitat = "Terrestre";


	  print ("""
	  El nombre del animal es: ${elefante.nombre}
	  Su tipo de alimentación es: ${elefante.alimentacion}
	  Su tipo de desarrollo embrionario es: ${elefante.nacimiento}
	  El habitat donde se encuentra es: ${cocodrilo.habitat}

	  """);

	  Cerdo cerdo = new Cerdo();
	  cerdo.nombre = "cerdo";
	  cerdo.alimentacion =  "Omnivoro";
	  cerdo.nacimiento = "Vivíparo";
	  cerdo.habitat = "Terrestre";  


	  print("""
	  El nombre del animal es: ${cerdo.nombre}
	  Su tipo de alimentación es: ${cerdo.alimentacion}
	  Su tipo de desarrollo embrionario es: ${cerdo.alimentacion}
	  El habitat donde se encuentra es: ${cerdo.habitat}

	  """);

	  Tiburon tiburon = new Tiburon();
	  tiburon.nombre = "Tiburon";
	  tiburon.alimentacion = "Carnivoro";
	  tiburon.nacimiento = "Vivíparo";
	  tiburon.habitat = "Acuático";


	  print("""
	  El nombre del animal es: ${tiburon.nombre}
	  Su tipo de alimentación es: ${tiburon.alimentacion}
	  Su tipo de desarollo embrionario es: ${tiburon.nacimiento}
	  El habitat donde se encuentra es: ${tiburon.habitat}

	  """);

	}

	   class Animal{
	     String? nombre;}
	   class Carnivoro extends Animal{
	      String? alimentacion;}
	   class Herviboro extends Animal{
	      String? alimentacion;}
	   class Omnivoro extends Animal{
	     String? alimentacion;}
	   class Cocodrilo extends Carnivoro{
	     String? nacimiento;
	     String? habitat;}
	  class Elefante extends Herviboro{
	    String? nacimiento;
	    String? habitat;}
	  class Cerdo extends Omnivoro{
	    String? nacimiento;
	    String? habitat;}
	  class Tiburon extends Carnivoro{
	    String? nacimiento;
	    String? habitat;}   

### EMPRESAS 
		void main(){
	    Empresa empresa1 = new Empresa(pais:'Argentina', numero:1043660098, oficina:'Advantice');
	    Empresa empresa2 = new Empresa(pais:'Colombia', numero: 3242828122, oficina:'Lenovo');


	   print("""
	    Usuarios de Empresas
	    1° Empresa:

	      Pais: ${empresa1.pais}.
	      Identificacion: ${empresa1.numero}.
	      Oficina: ${empresa1.oficina}.
	      Codigo: ${empresa1.generarCodigo()}
	  """);
              empresa1.cantCaracteres();
  

	     print("""
	    2° Empresa:
	      Pais: ${empresa2.pais}.
	      Identificacion: ${empresa2.numero}.
	      Oficina: ${empresa2.oficina}

	      codigo: ${empresa2.generarCodigo()}
	  """);
	  
	      
	     empresa2.cantCaracteres();
	  }


	 class Empresa{
	    String? pais, oficina;
	    int? numero;
	 Empresa({this.pais, this.numero, this.oficina});

	  String? generarCodigo(){
	  String? paisCod = pais!.substring(0,3);
	  int? cantoff = oficina?.length; 
	  int? poffice = cantoff! - 3; 
	  String? oficinaCod = oficina!.substring(poffice,cantoff);
	  String? cantnum = numero.toString();
	  String? nume = cantnum.substring(0,4);
	  String? codigo = '$paisCod$oficinaCod$nume';
	  return codigo;  
	    }

	 void cantCaracteres(){
	   int? crtpais = pais!.length; 
	   int? cantoff= oficina!.length;
	   String? crtnumero = numero.toString();
	   int? numerocrt = crtnumero.length; 

	   print("""
	  ----------------------------------------
	    caracteres de oficina son: $cantoff.
	    caracteres de pais: $crtpais.
	    caracteres de numero: $numerocrt.
	   ----------------------------------------
	""");
	}
	}
### Ejericicio practica 2 (length/substring/ToString)
	    void main (){

	  Inscripcion inscripcion1 = Inscripcion (nombre: 'Juan', apellido: 'Gallego', telefono: 3024550070);
	  Inscripcion inscripcion2 = Inscripcion (nombre: 'Zharick', apellido: 'Donado', telefono: 3242828122);

	  print("""
	  1° Usuario:
	  El nombre del usuario es: ${inscripcion1.nombre}
	  El apellido es: ${inscripcion1.apellido}
	  el telefono es: ${inscripcion1.telefono}

	  Su codigo generado es: ${inscripcion1.generarCodigo()}


	  """);
	  inscripcion1.cantCaracteres();


	   print("""
	  2° Usuario:
	  El nombre del usuario es: ${inscripcion2.nombre}
	  El apellido es: ${inscripcion2.apellido}
	  el telefono es: ${inscripcion2.telefono}

	  Su codigo generado es: ${inscripcion2.generarCodigo()}

	  """);
	 inscripcion2.cantCaracteres();
	}

	class Inscripcion{
	  String? nombre;
	  String? apellido;
	  int? telefono;
	Inscripcion({this.nombre, this.apellido, this.telefono});

	String generarCodigo(){
	  String? nombreCod = nombre!.substring(0,3);
	  String? apellidoCod = apellido!.substring(0,3);
	  String? numeroCod = telefono!.toString();
	  String? telefonoCod = numeroCod.substring(0,3);
	  String? codigo = '$nombreCod,$apellidoCod,$telefonoCod';
	  return codigo; 
	}
	void cantCaracteres(){
	  int? cantnombre = nombre!.length;
	  int? cantapellido = apellido!.length;
	  String? cantnumero = telefono!.toString();
	  int? cantelefono = cantnumero.length; 

	 print 
	   ("""
	   --------------------------------------
	 La cantidad de caracteres en nombre es: $cantnombre
	 La cantidad de caracteres en apellido es: $cantapellido
	 La cantidad de caracteres en telefono es: $cantelefono
	 ---------------------------------------
	 """);

	}

	}
### Practica modificaciones #3
	void main (){

	  Inscripcion inscripcion1 = Inscripcion (nombre: 'Juan', apellido: 'Gallego', telefono: 3024550070);
	  Inscripcion inscripcion2 = Inscripcion (nombre: 'Zharick', apellido: 'Donado', telefono: 3242828122);

	  print("""
	  1° Usuario:
	  El nombre del usuario es: ${inscripcion1.nombre}
	  El apellido es: ${inscripcion1.apellido}
	  el telefono es: ${inscripcion1.telefono}

	  Su codigo generado es: ${inscripcion1.generarCodigo()}


	  """);
	  inscripcion1.cantCaracteres();


	   print("""
	  2° Usuario:
	  El nombre del usuario es: ${inscripcion2.nombre}
	  El apellido es: ${inscripcion2.apellido}
	  el telefono es: ${inscripcion2.telefono}

	  Su codigo generado es: ${inscripcion2.generarCodigo()}

	  """);
	 inscripcion2.cantCaracteres();
	}

	class Inscripcion{
	  String? nombre;
	  String? apellido;
	  int? telefono;
	Inscripcion({this.nombre, this.apellido, this.telefono});

	String generarCodigo(){
	  int? nombreA = nombre?.length;
	  int? nombreB = nombreA! - 2;
	  String? nombreCod = nombre!.substring(nombreB, nombreA);
	  int? apellidoA = apellido?.length;
	  int? apellidoB = apellidoA! - 3;
	  String? apellidoCod = apellido!.substring(apellidoB,apellidoA);
	  String? numeroCod = telefono!.toString();
	  String? telefonoCod = numeroCod.substring(0,3);
	  String? codigo = '$nombreCod$apellidoCod$telefonoCod';
	  return codigo; 
	}
	void cantCaracteres(){
	  int? cantnombre = nombre!.length;
	  int? cantapellido = apellido!.length;
	  String? cantnumero = telefono!.toString();
	  int? cantelefono = cantnumero.length; 

	 print 
	   ("""
	   --------------------------------------
	 La cantidad de caracteres en nombre es: $cantnombre
	 La cantidad de caracteres en apellido es: $cantapellido
	 La cantidad de caracteres en telefono es: $cantelefono
	 ---------------------------------------
	 """);

	}

	}
	
### Lista 
	void main(){

	  List listapais = ['Argentina', 'Colombia', 'Mexico']; 
	  List listanumero = [1043660098, 3242828122, 8566820]; 
	  List listaoficina = ['advantice', 'Lenovo', 'apple'];

	  for (int i = 0; i < 3; i++){

	    Empresa empresa = Empresa(pais:listapais[i],numero:listanumero[i],oficina:listaoficina[i]);
	    print ('''
	    El codigo de la empresa es: ${empresa.generarCodigo()}
	    el pais es: ${empresa.pais}
	    el numero es: ${empresa.numero}
	    la oficia es: ${empresa.oficina}
		  ''');

	    empresa.cantCaracteres();

	  }
	}
	 class Empresa{
	    String? pais, oficina;
	    int? numero;
	 Empresa({this.pais, this.numero, this.oficina});

	  String? generarCodigo(){
	  String? paisCod = pais!.substring(0,3);
	  int? cantoff = oficina?.length; 
	  int? poffice = cantoff! - 3; 
	  String? oficinaCod = oficina!.substring(poffice,cantoff);
	  String? cantnum = numero.toString();
	  String? nume = cantnum.substring(0,4);
	  String? codigo = '$paisCod$oficinaCod$nume';
	  return codigo;  
	    }

	 void cantCaracteres(){
	   int? crtpais = pais!.length; 
	   int? cantoff= oficina!.length;
	   String? crtnumero = numero.toString();
	   int? numerocrt = crtnumero.length; 

	   print("""
	  ----------------------------------------
	    caracteres de oficina son: $cantoff.
	    caracteres de pais: $crtpais.
	    caracteres de numero: $numerocrt.
	   ----------------------------------------
	""");
	}
	}
	
## ejercicio de herencia 
	   main(){

	  Chofer chofer = Chofer();
	  chofer.id = 12345;
	  chofer.name = 'Andy';
	  chofer.salario = 1100;
	  chofer.vehiculoAsignado = 'Toyota Supra';
	  chofer.calcularSalario();

	  print("""
	  el nombre del chofer es: ${chofer.name}
	  el salario es: ${chofer.salario}
	  el vehiculo asignado es: ${chofer.vehiculoAsignado}
	  """);
	}


	class Empleado{
	  int? id;
	  String?  name;
	  double? salario;

	  void calcularSalario(){
	    print('El salario de $name es $salario');
	  }
	}

	// Hereda de Empleado
	class Chofer extends Empleado{
	  String? vehiculoAsignado;

	}

### ejercicio clase abstracta 
	void main(){
	  Vaca vaca1 = Vaca();
	  Gato gato2 = Gato(); 

	  Perro perro3 = Perro();
	  perro3.nombre = "Astro";

	  print("Sonido de los animales"); 
		vaca1.emitirSonido();
		gato2.emitirSonido();
		perro3.emitirSonido();

	  print("El IMC (indice de masa corporal) del perro ${perro3.nombre} es de:");
	  Carnivoro.imc(37,6); 
	}
	abstract class Animal{
	  void emitirSonido(); 
	}
	class Carnivoro{
	  String? nombre;
	  static void imc (a, b) => print (a * b);
	}
	class Vaca implements Animal{
	    @override 
	  void emitirSonido() => print ("La vaca hace MUUUUUUUUU"); 
	}
	class Gato implements Animal{
	    @override
	   void emitirSonido() => print("El gato hace MIAUUUUUU");
	}
	class Perro extends Carnivoro implements Animal{
	  @override
	  void emitirSonido() => print("El perro hace GUAU GUAU"); 
	}
	
	
### Accesorio 

void main(){
   
 Car car = Car (); 
 Accesorio accesorio1 = Accesorio ("Polarizado"); 
 Accesorio accesorio2 = Accesorio ("Rines");
 Accesorio accesorio3 = Accesorio ("Luces"); 
 car.placa = "ZYD1923";

 car.setAccesorio(accesorio1);
 car.setAccesorio(accesorio2); 
 car.setAccesorio(accesorio3); 
  
  
}
class Car{
 String? placa;
  
  List<Accesorio> _accesorio = []; 
  void setAccesorio(Accesorio accesorio){
    _accesorio.add(accesorio); 
  } 
  List<Accesorio> getAccesorio(){
    return _accesorio; 
  }
  }

class Accesorio{
  String? nombre; 
  Accesorio(this.nombre); 
}

