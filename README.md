# JavaInterfaz

   interfaz en java

una interfaz en Java generalmente implica diseñar una interfaz gráfica de usuario (GUI) que los usuarios puedan interactuar. Puedes crear una interfaz gráfica en Java utilizando varias tecnologías, pero una de las formas más comunes es utilizando la biblioteca Swing. A continuación, te proporciono un ejemplo básico de cómo crear una ventana de interfaz gráfica en Java utilizando Swing:

import javax.swing.JFrame;
import javax.swing.JLabel;
import javax.swing.JButton;
import javax.swing.JTextField;
import java.awt.event.ActionEvent;
import java.awt.event.ActionListener;

public class InterfazEjemplo {
    public static void main(String[] args) {
        // Crear una ventana
        JFrame ventana = new JFrame("Mi Primera Interfaz");
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

