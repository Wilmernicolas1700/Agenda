### Agenda
agenda donde llevare todo mi progreso del curso  ADSO

### 9-10 de agosto
### Hoja de vida por githud
primero que todo debemos crear una cuenta de githud la cual va a ser muy necesaria de ahora en adeante ya que va a ser como nuestro portaforio en esto de la programacion 
luego que tengamos nuestra cuenta de githud debemos editar nuestro perfil dando algunos de nuestros principales datos personalas 
**nombre,** **ubicación,** **tus habilidades,** **como te pueden encotrar por las redes sociales** 
luego para subir nuestra hoja de vida debemos crear un repositorio
### como crear un repositorio 
para crear uno debemos buscar es donde diga **repositorio** y tenemos que crear un nuevo repositrio, luego le colocamos nombre a nuestro repositorio y lo colocamos en publico ya que así es como debemos de trabajar en estos momentos, debemos de crear nuestro repositorio por **README**   

### EJEMPLO DE LA HOJA DE VIDA

### Hoja de vida 
Wilmer Nicolas Carmona Alvarez

<a href="https://ibb.co/52h1btW"><img src="https://i.ibb.co/52h1btW/xd.jpg" alt="xd" border="0"></a>
### Perfil
 Soy una persona que es caracterizado por ser responsable, de buenos modales y con altas ganas de superarse como persona cada día.
Cuento con la capacidad de adaptación y flexibilidad, siempre en disposición para el correcto cumplimiento de las funciones, cada día es un reto y mi día no se termina hasta cumplirlo
### Datos personales

- **Cédula de ciudadanía:** 1002303631
- **Fecha de nacimiento:** 17 de julio 2002
- **Lugar de nacimiento:** El Guamo Bolivar
- **Ciudad:** Malambo
- **dirección:** calle 7B 3SUR #79
- **E-mail:** wilmercarmona810@gmail.com
- **Estado civil:** soltero
 
### Formación académica
- **Titulación:** Bachiller técnico
- **Institución:** I.E.T.A Del Guamo

### 12 de agosto
### Resumen de la clase de excel

en la clase pasada aprendimos a activar el modo programador por excel para así comenzar a programar por medio de visual basic con los codigos requeridos para el programa
### Codigos aprendidos
**sud + nombre del rograma** = le da inicio y final al programa  
**Msgbox** = para mostrar el mensaje en la pantalla  
**a** (valor al numerico) asignar un valor a variable
### inicio y final
puedes empezar con sud y para terminar es end sud
### EJEMPLO DE LA CLASE DE ECXEL 

´´´´

sub sena

    nom = "Nicolas"
    msgbox nom
    num = 10
    msgbox num
    nom = "Sofia"
    msgbox "El nombre es " & nom

end sub

´´´´

### 26 de agosto
### CODIGO DE INGRESO
En esta clase debiamos crear un codigo  utilizando visual basic que permitiera calcular el valor a pagar por impuesto anual a una empresa 
### EJEMPLO 
´´´´
    
    Sub impuesto_empresa()

    ing_anual = InputBox("Ingrese su ingreso anual: ")

    If ing_anual >= 0 And ing_anual < 1000 Then
        MsgBox "No paga impuesto"
    Else
        If ing_anual >= 1001 And ing_anual < 10000 Then
            aum_imp = ing_anual * 0.05
            MsgBox "Impuesto a pagar: " & aum_imp
        Else
            If ing_anual >= 10001 And ing_anual < 100000 Then
                aum_imp = ing_anual * 0.1
                MsgBox "Impuesto a pagar: " & aum_imp
            Else
                If ing_anual >= 100001 And ing_anual < 1000000 Then
                    aum_imp = ing_anual * 0.15
                    MsgBox "Impuesto a pagar: " & aum_imp
                Else
                    If ing_anual >= 1000001 And ing_anual < 10000000 Then
                        aum_imp = ing_anual * 0.2
                        MsgBox "Impuesto a pagar: " & aum_imp
                    Else
                        If ing_anual > 10000001 Then
                            aum_imp = ing_anual * 0.25
                            MsgBox "Impuesto a pagar: " & aum_imp
                        Else
                            MsgBox "No se puede"    
                        End If
                         
                    End If
                        
                End If
            
            End If

        End If

    End If

    End Sub
´´´´

### 29 DE AGOSTO
### Codigo de registro de un carro
En esta clase nos enseñaron a como mover datos en excel de una hoja a otra hoja y de una celda a otra celda, para esto el instructor nos colocó un ejercicio de hacer un registro de carros donde en la primera hoja tenias que registrar tu carro y luego de registrarlo los datos se pasaban a la otra hoja de datos de excel gracias al programa que ejecutamos 

### EJEMPLO DEL PROGRAMA
´´´´

    Sub save()
        fila = datos.Cells(1, 8)
        datos.Cells(fila, 2) = registro.Cells(5, 4)
        datos.Cells(fila, 3) = registro.Cells(7, 4)
        datos.Cells(fila, 4) = registro.Cells(9, 4)
        datos.Cells(fila, 5) = registro.Cells(11, 4)
        MsgBox "Datos Guardados"
        datos.Cells(1, 8) = fila + 1
        
    End Sub

    ´´´´


Este codigo es el de pasar los datos ingresados en la primera hoja para la segunda hoja donde se tenias que guardar 

´´´´

Sub registrar()

cont = 3
    
    For w = 1 To 10
        name = InputBox("Ingrese su nombre:")
        datos.Cells(conta, 2) = name
        conta = conta + 1
    Next w
    
End Sub

´´´´

### 31 de agosto
### Codigo para un recaudo de un evento estudiantil 
Para realizar este codigo debiamos hacer un taller que nos dejó el intructor el cual decia:
En una entidad educativa con 7500 estudiantes se requiere realizar una recolecta para sufragar los gastos de un evento organizado por el colegio.

Se requiere que el programa entregue la siguiente información:

Total Recaudado por los estudiantes de todo el colegio.
Valor del recaudo promedio para los estudiantes que aportaron dinero.
Número de estudiantes que aportaron dinero a la recolecta.
Número de estudiantes que NO colaboraron.
Cantidad de estudiantes que aportaron valores superiores a $10.000

debiamos buscar la logica nostros mismos de como realizar eso ese día me fue muy mal tratando de buscar esa logica, así que me tuve que guiar de la logica de un compañero 

### EJEMPLO DEL PROGRAMA

´´´´

Sub eventoescolar()
    
    abono = 0
    no_abono = 0
    cant_sup = 0
    total_recaudado = 0
    
    For a = 1 To 2
        dinero_rec = Int(InputBox("Cuanto va a abonar?"))
        If dinero_rec > 0 Then
            abono = abono + 1
            total_recaudado = total_recaudado + dinero_rec
            If dinero_rec >= 10000 Then
                cant_sup = cant_sup + 1
            End If
        Else
            no_abono = no_abono + 1
        End If
    Next a
    
    prom = total_recaudado / abono
    MsgBox "El total recaudado es de $" & total_recaudado
    MsgBox "El promedio del recaudo es de $" & prom
    MsgBox "La cantidad de estudiantes que donaron " & "(" & abono & ")" & " Estudiantes"
    MsgBox "La cantidad de estudiantes que no donaron " & "(" & no_abono & ")" & " Estudiantes"
    MsgBox "Los estudiantes que aportaron una cantidad superior a $10.000:   " & "(" & cant_sup & ")" & " Estudiantes"
        
End Sub

´´´´

### 02 de septiembre 
### Como seleccionar caracteres de una palabra por medio de un programa
En esta clse nos enseñaron como seleccionar caracteres de alguna frase por medio de un programa y para hacer eso nos mandaron a hacer un programa que permitiera separar las dos ultimas letras de algunos nombres 
### EJEMPLO DEL PROGRAMA

´´´´

    Sub ultimador()


        For a = 2 To 21
            nom = lista.Cells(a, 1)
            ult = Len(nom) - 1
            lista.Cells(a, 2) = Mid(nom, ult, 2)
        Next a
        
    End Sub


´´´´