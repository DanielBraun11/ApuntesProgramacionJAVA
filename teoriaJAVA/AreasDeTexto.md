# Áreas de Texto - JTextArea
**IMPORTANTE** los ejemplos de este apartado estan relacionados con las Ventanas(JFrame) y Paneles(JPanel) de los apuntes anteriores.
### Creación de un Área de Texto
```java
JTextArea areaTexto = new JTextArea();
```
### Dar tamaño y posición
Si tenemos desactivado el diseño del panel
```java
panel.setLayout(null); //descativar diseño
```
Debemos indicar el tamaño que tenga nuestro área de texto y la posición(ubicación) en la que se encuentre en el panel:
```java
areaTexto.setBounds(20,20,300,200); //(x,y,ancho,alto)
```
### Establecer texto que queramos
```java
areaTexto.setText("Escribe el texto: ");
```
### Añadir el área de Texto a un panel
```java
panel.add(areaTexto);
```
### Añadir texto al área de texto
Añadiremos una cadena de texto al que ya pueda tener el área
```java
areaTexto.append(""); //Añade mas texto al area
```
### Conceder permisos de edicion sobre el área
```java
areaTexto.setEditable(true); //Editable
areaTexto.setEditable(false); //No editable
```
### Obtener el texto que hay en el área
```java
String texto = areaTexto.getText();
System.out.println(texto);
System.out.println(areaTexto.getText());
```
