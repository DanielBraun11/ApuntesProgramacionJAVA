# Método Constructor
Es un método especial de una clase que se invoca siempre que se crea un objeto de esa clase.
Cuando se crea un objeto ocurren 3 cosas:
- Se asigna memoria para el objeto
- Se inicializan los atributos de ese objeto
- Se invoca al constructor de la clase que puede ser uno entre varios.
```java
Persona persona1 = new Persona();   //Persona() es la llamada al método constructo de la clase Persona
```
## Características de los Constructores
- Tienen el mismo nombre de la clase
- No devuelven ningun valor
- Deben declararse como públicos
### Ejemplo
```java
public class Persona{
    String nombre;
    int edad;

    public Persona(String n, int e){
        nombre = n;
        edad = e;
    }

    public void mostrarDatos(){
        System.out.println("Nombre: " + nombre);
        System.out.println("Edad: " + edad);
    }

    public static void main(String[] args) {
        Persona persona1 = new Persona("Daniel",20);

        persona1.mostrarDatos();
    }
}
```


