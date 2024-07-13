# Diagrama de clase
``` mermaid
classDiagram
    Usuario "1..*" -- "0..*" Actividad: is associated with
    Actividad "1..*" -- "1..*" Categoria: is associated with
    Actividad "1..*" *-- "1" Meta: has
    Actividad "1" o-- "1" Estado: has
    Actividad "1..*"o-- "1..*" Notificación: use
    Notificación "1..*" o-- "1" Calendario: use
    Hábitos --|> Actividad: implements
    Usuario: int id
    Usuario: string nombre
    Usuario: string email
    Hábitos: int id
    Actividad: int id
    Actividad: string nombre
    Actividad: string descripción



```
