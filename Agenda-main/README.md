### Agenda
agenda de apuntes
### Resumen de la clase
en la clase pasada aprendimos a activar el modo programador por excel para así comenzar a programar por medio de visual basic con los codigos requeridos para el programa
### Codigos aprendidos
**sud + nombre del rograma** = le da inicio y final al programa  
**Msgbox** = para mostrar el mensaje en la pantalla  
**a** (valor al numerico) asignar un valor a variable
### inicio y final
puedes empezar con sud y para terminar es end sud
### ejemplo
sud ejemplo()  
a = 10  
b = Sofia  
c = Nicolas  
end sud  

### Trabajo 26 de agosto

´´´´

    Sub ejercicio()
        ing_a = InputBox("escribir el ingreso anual de la empresa :")
        
        If ing_a >= 0 And ing_a < 1000 Then
            MsgBox "la empresa no paga"
        Else
        If ing_a >= 1001 And ing_a < 10000 Then
            Total = ing_a * 0.05
            MsgBox "su impuesto es de: " & Total
        Else
            If ing_a >= 10001 And ing_a < 100001 Then
            Total = ing_a * 0.1
            MsgBox "su impuesto es de: " & Total
            Else
                If ing_a >= 100001 And ing_a < 1000000 Then
                    Total = ing_a * 0.15
                    MsgBox "su impuesto es de: " & Total
                Else
                    If ing_a >= 1000001 And ing_a < 10000000 Then
                        Total = ing_a * 0.2
                        MsgBox "su impuesto es de: " & Total
                    Else
                        If ing_a >= 10000001 Then
                            Total = ing_a * 0.25
                            MsgBox "su impuesto total es de: " & Total
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
