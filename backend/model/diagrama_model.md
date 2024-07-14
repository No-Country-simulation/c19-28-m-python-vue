# Diagrama de clase
``` mermaid
classDiagram
    Usuario "1..*" -- "0..*" Actividad: is associated with
    Actividad "1..*" -- "1..*" Categoria: is associated with
    Actividad "1..*" *-- "1" Meta: has
    Actividad "1..*"o-- "1..*" Notificación: use
    Hábitos --|> Actividad: implements
    Usuario: int id
    Usuario: string nombre
    Usuario: string email
    Hábitos: int id
    Actividad: int id
    Actividad: string nombre
    Actividad: string descripción
    Actividad: datatime fecha_inicio
    Actividad: datatime fecha_fin
    Actividad: string tipo
    Actividad: string plazo
    Actividad: estado
    Categoria: int id
    Categoria: string nombre
    Categoria: string descripción
    Meta: int id
    Meta: string descripción
    Meta: boolean cumplida
    Notificación: int id
    Notificación: string mensaje
    Notificación: datatime fecha
    Notificación: boolean leida



```

