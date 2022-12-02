
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
	
### json 1 
	import 'package:http/http.dart' as http; 
	import 'dart:convert' as convert; 

	void main() async {
	  final url = Uri.https('reqres.in','api/users/3');
	  final response = await http.get(url); 

	  if (response.statusCode == 200){
	    final json = convert.jsonDecode(response.body); 
	    print(json["data"]["email"]); 
	    print(json["data"]["first_name"]); 
	    print(json["support"]["url"]); 
	  }
	  else{
	     print('problemas encontrados');  
	  } 

	}

### json 2
	import 'package:http/http.dart' as http; 
	import 'dart:convert' as convert; 

	void main() async {
	  final url = Uri.https('jsonplaceholder.typicode.com' , 'posts/4');
	  final response = await http.get(url); 

	  if (response.statusCode == 200){
	    final json = convert.jsonDecode(response.body); 
	  print(json["userId"]); 
	  print(json["id"]); 
	  print(json["title"]); 
	  print(json["body"]); 
	  }
	  else{
	     print('problemas encontrados');  
	    }
	  } 
	  
### buho 

	import 'package:flutter/material.dart';

	void main(){
	     runApp(MyApp()); 
	}

	class MyApp extends StatelessWidget {
	  @override
	  Widget build(BuildContext context) {
	    return MaterialApp(
	      title: 'My application',
	      home: Scaffold(appBar: AppBar(title: Text('Aplicacion ventana')),
	      body: Column(
		children: [
		  SizedBox(height: 15.0),
		  Text('Zharick Donado', style: TextStyle(fontSize: 25.0),), 
		  SizedBox(height: 15.0), 
		  const Image(
	  image: NetworkImage('https://flutter.github.io/assets-for-api-docs/assets/widgets/owl.jpg', scale: 2.0),
	),
	      SizedBox(height: 15.0),
	      Text('zharickdonado848@gmail.com', style: TextStyle(fontSize: 20.0),),
	      SizedBox(height: 15.0),
	      Row(
		mainAxisAlignment: MainAxisAlignment.spaceEvenly,
		children:[
	      Icon(
		  Icons.facebook,
		  color: Colors.blue,
		  size: 24.0,
		  semanticLabel: 'Text to announce in accessibility modes',
		),
	      Icon(
		  Icons.speaker_notes_sharp,
		  color: Colors.orange,
		  size: 30.0,
		),
	      Icon(
		  Icons.send_and_archive_outlined,
		  color: Colors.blue,
		  size: 36.0,
		),
	    ],

	      )
		],
	      )
	    ),
	  );
	  }
	}
	
### main 
		import 'package:flutter/material.dart';
	import 'models/user.dart';
	import 'package:http/http.dart' as http;
	import 'widgets/template.dart';

	void main() => runApp(MyApp());

	class MyApp extends StatelessWidget {
	  @override
	  Widget build(BuildContext context) {
	    return MaterialApp(
	      title: 'My application',
	      home: Scaffold(
		appBar: AppBar(
		    title: Text('Perfil de usuario'),
		    backgroundColor: Colors.deepPurple[600]),
		    backgroundColor: Colors.grey[400],
		body: FutureBuilder<User>(
		  future: getUser(),
		  builder: (context, snapshot) {
		    if (snapshot.connectionState == ConnectionState.done) {
		      User user = snapshot.data as User;
		      return Template(user: user);
		    }
		    return Center(child: CircularProgressIndicator());
		  },
		),
	      ),
	    );
	  }

	  Future<User> getUser() async {
	    final url = Uri.https('reqres.in', '/api/users/6');
	    final response = await http.get(url);
	    return User(response.body);
	  }
	}


### user dart
	import 'dart:convert' as convert;

         class User {
	  String? nombre;
	  String? avatar;
	  String? email;

	  User(String json) {
	    final jsonResponde = convert.jsonDecode(json);
	    nombre = jsonResponde["data"]["first_name"];
	    avatar = jsonResponde["data"]["avatar"];
	    email = jsonResponde["data"]["email"];
	  }
	}
### template
		 import 'package:flutter/material.dart';
	import 'package:sena/models/user.dart';

	class Template extends StatelessWidget {
	  const Template({
	    Key? key,
	    required this.user,
	  }) : super(key: key);

	  final User user;

	  @override
	  Widget build(BuildContext context) {
	    return Column(
	      children: [
		SizedBox(height: 15.0),
		Text(user.nombre!, style: TextStyle(fontSize: 20.0)),
		SizedBox(height: 15.0),
		Image(
		  image: NetworkImage(user.avatar!),),
		SizedBox(height: 15.0),
		Text(user.email!, style: TextStyle(fontSize: 20.0)),
		SizedBox(height: 15.0),
		Row(
		  mainAxisAlignment: MainAxisAlignment.spaceEvenly,
		  children: [
		    Icon(Icons.person_add_alt_sharp,
			color: Colors.black,
			size: 40.0,
			semanticLabel: 'Text to announce in accessibility modes'),
		    Icon(Icons.favorite_rounded, color: Colors.red, size: 40.0),
		    Icon(Icons.insert_comment_rounded, color: Colors.black, size: 40.0),
		  ],
		)
	      ],
	    );
	  }
	}
	
### Nuevo add

	  main: 
	      import 'package:flutter/material.dart';
	import 'package:sena/widgets/menulateral.dart';
	import 'models/user.dart';
	import 'package:http/http.dart' as http;
	import 'widgets/template.dart';
	void main() => runApp(Sena());

	class Sena extends StatelessWidget {
	  @override
	  Widget build(BuildContext context) {
	    return MaterialApp(
	      title: 'My application',
	      home: Scaffold(
		  appBar: AppBar(title: const Text('Chats de inicio'), 
		  Drawer: MenuLateral(),
		  leading: IconButton(icon: const Icon(Icons.menu), onPressed: () {},),
		  actions: <Widget>[
		  IconButton(
		    icon: Icon(Icons.find_in_page_rounded),
		    onPressed: () {},),
		    IconButton(
		    icon: Icon(Icons.settings),
		    onPressed: () {},
		    ),
		   IconButton(
		    icon: Icon(Icons.settings),
		    onPressed: () {},
		    ),
		  ],

		  backgroundColor: Colors.green),
		  backgroundColor: Colors.grey[300],
		  body: FutureBuilder<List<User>>(
		    future: getData(),
		    builder: (context, snapshot) {
		      if (snapshot.connectionState == ConnectionState.done) {
			List<User> users = snapshot.data!;
			return ListView.builder(
			    itemCount: users.length,
			    itemBuilder: (BuildContext context, index) {
			      final user = users[index];
			      return ItemData(user: user);
			    });
		      }
		      return const Center(child: CircularProgressIndicator());
		    },
		  )),
	    );
	  }

	  Future<List<User>> getData() async {
	    final url = Uri.https('reqres.in', '/api/users');
	    final response = await http.get(url);
	    return userFromJson(response.body);
	  }
	  }
	  
### menu lateral 
	   import 'package:flutter/material.dart';

	class MenuLateral extends StatelessWidget{

	  @override
	  Widget build(BuildContext context) {
	    return new Drawer(
	      child: ListView(
		children: <Widget>[
		  new UserAccountsDrawerHeader(
		      accountName: Text("CODEA APP"),
		      accountEmail: Text("informes@gmail.com"),
		    decoration: BoxDecoration(
		      image: DecorationImage(
			  image: NetworkImage("https://dominio.com/imagen/recurso.jpg"),
			fit: BoxFit.cover
		      )
		    ),
		  ),
		  Ink(
		    color: Colors.indigo,
		    child: new ListTile(
		      title: Text("MENU 1", style: TextStyle(color: Colors.white),),
		    ),
		  ),
		  new ListTile(
		    title: Text("MENU 2"),
		    onTap: (){},
		  ),
		  new ListTile(
		    title: Text("MENU 3"),
		  ),
		  new ListTile(
		    title: Text("MENU 4"),
		  ) ],
	      ) ,
	    );
	  }
	}

### template 

	   import 'package:flutter/material.dart';
	import 'package:sena/models/user.dart';

	class ItemData extends StatelessWidget {
	  final User user;
	  const ItemData({
	    Key? key,
	    required this.user,
	  }) : super(key: key);

	  @override
	  Widget build(BuildContext context) {
	    return Column(
	      children: [
		ListTile(
		  title: Text('${user.firstName!} ${user.lastName!}'),
		  subtitle: Text(user.correoElectrnico!),
		  leading: CircleAvatar(backgroundImage: NetworkImage(user.avatar!),),
		  trailing: const Icon(Icons.arrow_forward_ios,color: Colors.blue,
	),
		),
		Divider(),
	      ],
	    );
	  }
	}
	
   
   user:
	   import 'dart:convert';
	import 'package:sena/main.dart';

	List<User> userFromJson(String str) => List<User>.from(json.decode(str)['data'].map((x) => User.fromJson(x)));

	class User {
	  User({
	    this.correoElectrnico,
	    this.firstName,
	    this.lastName,
	    this.avatar,
	  });

	  String? correoElectrnico;
	  String? firstName;
	  String? lastName;
	  String? avatar;

	  factory User.fromJson(Map<String, dynamic> json) => User(
		correoElectrnico: json["email"],
		firstName: json["first_name"],
		lastName: json["last_name"],
		avatar: json["avatar"],
	      );
	}
### html
 
	  !DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1.0">
	    <title>Vision</title>
	</head>
	<body>
	    <h1>Mision</h1>
	    <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Porro molestias distinctio dolores quidem, provident vitae a repudiandae rem ullam tempore explicabo quam commodi neque magni veniam consectetur. Laborum, dolor id?</p>
	    <body style="background-color:bisque;">
	    <img src="https://tresubresdobles.com/wp-content/uploads/2019/08/skft-912381dcd5b2c45c4a9ce8acf32cfd8c-768x961.jpg" width="300" height="300"/>
	    <h3>Menu</h3>
	    <a href="index.html">Inicio<br></a>
	    <a href="mision.html">mision<br></a>
	    <a href="vision.html">vision<br></a>

	    </body>
	</body>
	</html>
	

### HTML VETERINARIA INDEX

		<!DOCTYPE html>
		<html lang="es-co">
		<head>
		    <meta charset="UTF-8">
		    <link rel="stylesheet" href="style.css">
		    <title>Caninos</title>
		</head>
		<body>
		<main>
		    <header><img src="animales.png" alt="imagen" ></header>
		    <nav>
			<ul>
			    <li>Servicios</li>
			    <li>Productos</li>
			    <li>Guarderia</li>
			    <li>Alimentos </li>
			</ul>
		    </nav>
		    <section>
		    <article class= "arriba">
			<h1>Cuidados y educacion para su perro</h1>
			<p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Soluta ratione autem corporis voluptas fuga perferendis sed fugit delectus nostrum quas? Esse quisquam quibusdam autem sint officiis, est ducimus eaque. Esse!</p>
			<img src="/perritozs.png" alt="imagen">
		    </article>
		    <article class= "abajo">
			<h1>salir de viaje con tu mascota</h1>
			<p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Placeat non veritatis ad suscipit, recusandae deserunt maxime nam, numquam animi, modi consequatur dolorem! Voluptatibus obcaecati molestias qui dignissimos, laboriosam quos illo!</p>
			<img src="/perritoz.png" alt="imagen">
		    </article>
		    </section>
		    <aside>
			<header><p>Solicitar cita médica</p></header>
		    </aside>
		    <footer><br>
			<p>Contactos</p>
			<p>Linea gratuita 018000-00001</p>
			<p>Correo:preguntas@caninosyfelinos.com</p>
		    </footer>
		</main>
		</body>
		</html>

### HTML VETERINARIA STYLE.CSS

	    main{
	    border: 1px solid rgb(255, 255, 255);
	    width: 1500px;
	    height: 1500px;
	    border-radius: 40px;
	    margin: auto;
	}

	header{
	    height: 235px;
	    border-top-left-radius: 40px;
	    border-top-right-radius: 40px;
	}

	img{
	    height: 250px;
	    width: 1500px;
	    }


	nav{

	    height: 130px;
	    border-bottom-left-radius: 40px;
	    border-bottom-right-radius: 40px;
	    margin-bottom: 2px;
	    background-color: #1c4a48;
	}
	ul li{
	    border-right: 1px solid white;
	    color: rgb(255, 255, 255);
	    display: inline-flex;
	    font-size: 55px;
	    font-family: Arial, Helvetica, sans-serif;
	    margin: 30px 30px 30px 40px;
	    padding-right: 40px;
	}

	section{

	    height: 900px;
	    width: 900px;
	    margin: 10px;
	    margin-left: 10px ;
	    margin-top: 30px;
	    float: left;
	}

	article{
	    border: 1px solid rgb(255, 255, 255);
	    background-color: #fbf5b9;
	    height: 370px;
	    margin-bottom: 70px;
	    margin-top: 0;
	    border-radius: 10px;
	    padding: 0 0 0 25px;

	}
	article img{
	    width: 252px;
	    float: right;
	    margin: 20px 25px 0 0;
	    border: 6px solid black;
	    border-radius: 30px;
	}
	article h1{
	    font-size: 40px;
	    margin: 15px 0 0 0 ;
	}
	article p {
	    display: inline-block;
	    width: 500px;
	    font-size: 32px;
	}
	.arriba{
	    border-radius: 45px 45px 0 0;
	}
	.abajo{
	    border-radius: 0 0 45px 45px;
	}

	aside{
	    border: 1px solid rgb(16, 112, 40);
	    height: 850px;
	    width: 520px;
	    display: inline-block;
	    margin-left: 25px;
	    margin-bottom: 10px;
	    margin-top: 30px;
	    border-radius: 50px;
	    background-color: #4a6e6e;

	}
	aside header{
	    height: 100px;
	}
	aside p{
	    font-size: 50px;
	    margin: auto;
	    display: flex;
	    align-items: center;
	    justify-content: center;
	    color: white;
	    background-color: #1c4a48;
	    height: 140px;
	    border-radius: 50px 50px 0 0 ;
	}
	footer{
	    height: 210px;
	    background-color: #1c4a48;
	    padding: 30px 0 0 0;
	    border-radius: 0 0 45px 45px;    
	}
	footer p{
	    color: white;
	    display: flex;
	    font-size: 39px;
	    justify-content: center;
	    align-items: center;
	    margin: 0;
	}


