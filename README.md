# JavaInterfaz
Editor.md
Editor Markdown en línea de código abierto.

En este ejemplo, hemos creado una interfaz gráfica simple con una ventana que contiene una etiqueta, un campo de texto y un botón. La etiqueta muestra un saludo, el campo de texto permite al usuario ingresar un nombre y el botón cambia el saludo en la etiqueta cuando se hace clic en él.
interfaz en java
​
Una interfaz en Java generalmente implica diseñar una interfaz gráfica de usuario (GUI) que los usuarios puedan interactuar. Puedes crear una interfaz gráfica en Java utilizando varias tecnologías, pero una de las formas más comunes es utilizando la biblioteca Swing. A continuación, te proporciona un ejemplo básico de cómo crear una ventana de interfaz gráfica en Java utilizando Swing:
​
importar javax.swing.JFrame;
importar javax.swing.JLabel;
importar javax.swing.JButton;
importar javax.swing.JTextField;
importar java.awt.event.ActionEvent;
importar java.awt.event.ActionListener;
​
public class InterfazEjemplo {
    público estático vacío principal (String [] argumentos) {
        // Crear una ventana
        JFrame ventana = new JFrame("Mi Primera Interfaz");
        ventana.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE); // Cierra la aplicación cuando se cierra la ventana
        ventana.setSize(400, 200); // Tamaño de la ventana (ancho, alto)
​
        // Crear un componente de etiqueta
        JLabel etiqueta = new JLabel("¡Hola, Mundo!");
        etiqueta.setBounds(150, 30, 200, 30); // Posición y tamaño (x, y, ancho, alto)
​
        // Crear un campo de texto
        JTextField campoTexto = nuevo JTextField();
        campoTexto.setBounds(150, 70, 150, 30);
​
        // Crear un botón
        Botón JButton = new JButton("Haz clic");
        botón.setBounds(150, 110, 100, 30);
​
        // Agregar un ActionListener al botón para manejar eventos de clic
        boton.addActionListener(nuevo ActionListener() {
            @Anular
interfaz en java

Una interfaz en Java generalmente implica diseñar una interfaz gráfica de usuario (GUI) que los usuarios puedan interactuar. Puedes crear una interfaz gráfica en Java utilizando varias tecnologías, pero una de las formas más comunes es utilizando la biblioteca Swing. A continuación, te proporciona un ejemplo básico de cómo crear una ventana de interfaz gráfica en Java utilizando Swing:

importar javax.swing.JFrame;
importar javax.swing.JLabel;
importar javax.swing.JButton;
importar javax.swing.JTextField;
importar java.awt.event.ActionEvent;
importar java.awt.event.ActionListener;

public class InterfazEjemplo {
public static void main(String[] args) {
// Crear una ventana
JFrame ventana = new JFrame(“Mi Primera Interfaz”);
ventana.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE); // Cierra la aplicación cuando se cierra la ventana
ventana.setSize(400, 200); // Tamaño de la ventana (ancho, alto)

    // Crear un componente de etiqueta
    JLabel etiqueta = new JLabel("¡Hola, Mundo!");
    etiqueta.setBounds(150, 30, 200, 30); // Posición y tamaño (x, y, ancho, alto)
    // Crear un campo de texto
    JTextField campoTexto = new JTextField();
    campoTexto.setBounds(150, 70, 150, 30);
    // Crear un botón
    JButton boton = new JButton("Haz clic");
    boton.setBounds(150, 110, 100, 30);
    // Agregar un ActionListener al botón para manejar eventos de clic
    boton.addActionListener(new ActionListener() {
        @Override
        public void actionPerformed(ActionEvent e) {
            etiqueta.setText("¡Hola, " + campoTexto.getText() + "!");
        }
    });
    // Agregar los componentes a la ventana
    ventana.add(etiqueta);
    ventana.add(campoTexto);
    ventana.add(boton);
    // Establecer el diseño de la ventana
    ventana.setLayout(null);
    // Hacer visible la ventana
    ventana.setVisible(true);
}
}

En este ejemplo, hemos creado una interfaz gráfica simple con una ventana que contiene una etiqueta, un campo de texto y un botón. La etiqueta muestra un saludo, el campo de texto permite al usuario ingresar un nombre y el botón cambia el saludo en la etiqueta cuando se hace clic en él.

Ejemplo
<enlace rel="hoja de estilo" href="editormd/css/editormd.css" />
<div id="editor-prueba">
    <textarea style="display:none;">### Editor.md

**Editor.md**: el editor de rebajas en línea integrable de código abierto, basado en CodeMirror, jQuery y Marked.
    </textarea>
</div>
<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/1.11.3/jquery.min.js"></script>
<script src="editormd/editormd.min.js"></script>
<tipo de script="texto/javascript">
    $(función() {
        var editor = editormd("editor de prueba", {
            // ancho: "100%",
            // altura: "100%",
            ruta: "editormd/lib/"
        });
    });
</script>
Copiar
Más ejemplos >>

Características
Admite Markdown estándar/CommonMark y GFM (GitHub Flavored Markdown);
Con todas las funciones: vista previa en tiempo real, carga de imágenes (entre dominios) , texto preformateado/bloques de código/inserción de tablas, plegado de código, reemplazo de búsqueda, solo lectura, temas, varios idiomas, L18n, entidades HTML, resaltado de sintaxis de código. ..;
Extras de Markdown: ToC de soporte (Tabla de contenido) , Emoji , listas de tareas , @Links ...;
Admite TeX (expresiones LaTeX, basadas en KaTeX) , diagrama de flujo y diagrama de secuencia de sintaxis extendida de Markdown;
Admite identificación, interpretación y filtrado de etiquetas HTML;
Admite el cargador de módulos AMD/CMD (Require.js y Sea.js) y complementos de editor personalizados/definidos;
Compatible con todos los principales navegadores (IE8+), Zepto.js y iPad compatibles;
Admite estilos de temas personalizados;
Descargar e instalar
Última versión: v1.5.0, Actualización: 2015-06-09



 


O instalación de NPM:

npm install editor.md



O instalación de Bower:

bower install editor.md




Registros de cambios:

CAMBIOS

Dependientes
Proyectos:

Código espejo
marcado
jQuery
FuenteImpresionante
github-markdown.css
KaTeX
Refael.js
prettify.js
diagrama de flujo.js
diagrama de secuencia.js
Prefijos.scss

Herramientas de desarrollo :

Código de estudio visual
Descaro/Scss
trago.js
Licencia
Editor.md sigue la licencia MIT y cualquiera puede utilizarla libremente.





Bifurcame en Github:







Usuarios

Contáctenos: editor.md@ipandao.com


Editor.md
Copyright © 2015-2019 Editor.md , licencia MIT.

Diseño y desarrollo por: Pandao     
