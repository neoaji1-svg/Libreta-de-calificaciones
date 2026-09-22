# Libreta-de-calificaciones

**Fecha:** 21/09/2026

## Contenido del Repositorio
Breve descripción general de lo que abarca esta práctica o laboratorio. En esta actividad se desarrollaron dos versiones del sistema **Libro de Calificaciones** en C# para consola, orientados a objetos. Se abordaron las estructuras de control repetitivas (`while`), evaluando tanto la repetición definida por contador como la repetición indefinida mediante el uso de un valor centinela (`-1`), además de la manipulación de tipos de datos enteros y de punto flotante (`double`) para el cálculo preciso de promedios.

## Tecnologías Utilizadas
* **Lenguaje / Framework:** C# (.NET Core / Aplicación de Consola)
* **IDE / Herramientas:** Visual Studio / Visual Studio Code, Git, GitHub

## Capturas de Pantalla y Problemas

### Interfaz Principal
![Salida General de Consola](img/interfaz_principal.png)

### Programa 1: Libro de Calificaciones con Repetición por Contador
* **Descripción de la solución:**  
  Se implementó la clase `LibroCalificaciones` que inicializa el nombre del curso a través de un constructor y expone la propiedad `NombreCurso`. El método `DeterminarPromedioClase()` utiliza una estructura de repetición `while` controlada por un contador que solicita exactamente 10 calificaciones al usuario. Suma los valores acumulados en la variable `total` y calcula el promedio con división entera.

### Programa 2: Libro de Calificaciones con Valor Centinela
* **Descripción de la solución:**  
  Se evolucionó la clase `LibroCalificaciones` para permitir el ingreso indeterminado de datos mediante un valor centinela (`-1`). El ciclo `while` finaliza únicamente cuando el usuario ingresa este valor de paro. Se incluyó una validación previa (`if (contadorCalif != 0)`) para evitar errores de división por cero y se aplicó conversión explícita (*casting*) a tipo `double` (`(double)total / contadorCalif`) junto con formato de salida (`{0:F2}`) para mostrar el promedio redondeado con dos decimales.

### Autor y Contexto
* **Nombre:** Neo Aji

* **Institución:** Universidad Tecnológica de Panamá (UTP)

* **Fecha de Realización:** 21/09/2026
   
### Referencias
* Documentación oficial de C# / .NET en Microsoft Learn

* Cómo programar en C# - Paul Deitel & Harvey Deitel

## Estructura de Carpetas o Directorios

```plaintext
mi-repositorio/
├── Librocalificaciones/            # Proyecto 1: Promedio de 10 calificaciones (Contador)
│   ├── LibroCalificaciones.cs      # Lógica de la clase e iteración por contador
│   ├── Program.cs                  # Punto de entrada y prueba de la solución
├── Librodecalificaciones_2/        # Proyecto 2: Promedio con valor centinela
│   ├── LibroCalificaciones.cs      # Lógica de la clase con centinela y casting double
│   ├── Program.cs                  # Punto de entrada y prueba de la solución
└── README.md                       # Documentación del proyecto
