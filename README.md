# Introducción a Arduino

Este es un breve repaso sobre Arduino, una plataforma de prototipado electrónico de código abierto que permite a los entusiastas de la electrónica y los programadores crear proyectos interactivos. Arduino se basa en hardware y software de fácil acceso y está diseñado para ser flexible y fácil de usar.

## Tabla de contenidos

1. [¿Qué es Arduino?](#qué-es-arduino)
2. [Componentes básicos](#componentes-básicos)
3. [Programación en Arduino](#programación-en-arduino)
4. [Estructura de un programa Arduino](#estructura-de-un-programa-arduino)
5. [Entradas y salidas](#entradas-y-salidas)
6. [Recursos adicionales](#recursos-adicionales)

## ¿Qué es Arduino?

Arduino es una plataforma de prototipado electrónico que consta de hardware y software. El hardware principal de Arduino es una placa de circuito impreso que incluye un microcontrolador y una serie de pines de entrada y salida. El software de Arduino proporciona un entorno de desarrollo integrado (IDE) basado en el lenguaje de programación C++ simplificado.

Arduino se utiliza ampliamente en proyectos de electrónica, robótica, domótica, arte interactivo y muchas otras aplicaciones. Es una herramienta accesible para principiantes y también es utilizada por profesionales y expertos en electrónica.

## Componentes básicos

Los componentes básicos utilizados en un proyecto de Arduino incluyen:

- **Placa Arduino**: La placa Arduino es el hardware principal que contiene el microcontrolador y los pines de entrada y salida.

- **Cables**: Se utilizan cables para realizar conexiones entre los componentes y la placa Arduino.

- **Resistencias**: Las resistencias se utilizan para limitar el flujo de corriente en un circuito.

- **LED**: Los LED (diodos emisores de luz) son componentes utilizados para emitir luz cuando se aplica una corriente eléctrica.

- **Sensores**: Los sensores se utilizan para detectar y medir variables del entorno, como temperatura, luz, movimiento, entre otros.

- **Actuadores**: Los actuadores son dispositivos que realizan una acción física en respuesta a una señal eléctrica, como motores, servomotores o relés.

Estos son solo algunos de los componentes básicos utilizados en proyectos de Arduino. La elección de los componentes dependerá del proyecto específico que desees realizar.

## Programación en Arduino

La programación en Arduino se realiza utilizando el lenguaje de programación C++ simplificado. El entorno de desarrollo integrado (IDE) de Arduino proporciona herramientas y funciones que simplifican la programación y la carga de código en la placa Arduino.

El lenguaje de programación de Arduino se basa en funciones, que se ejecutan en un bucle infinito. El bucle principal `loop()` se repite continuamente mientras la placa Arduino está encendida.

Aquí hay un ejemplo básico de un programa Arduino que hace parpadear un LED:

```cpp
// Definir el número de pin del LED
const int ledPin = 13;

// Configurar el pin del LED como salida
void setup() {
  pinMode(ledPin, OUTPUT);
}

// Encender y apagar el LED en un bucle infinito
void loop() {
  digitalWrite(ledPin,

 HIGH);   // Encender el LED
  delay(1000);                  // Esperar 1 segundo
  digitalWrite(ledPin, LOW);    // Apagar el LED
  delay(1000);                  // Esperar 1 segundo
}
```

Este programa utiliza la función `setup()` para configurar el pin del LED como salida y la función `loop()` para encender y apagar el LED en un bucle infinito.

## Estructura de un programa Arduino

Un programa Arduino típico consta de dos funciones principales:

- `setup()`: Esta función se ejecuta una vez al inicio del programa y se utiliza para configurar el entorno, como la inicialización de pines y variables.

- `loop()`: Esta función se ejecuta continuamente en un bucle infinito después de que se complete la función `setup()`. Aquí es donde se coloca el código principal del programa, que se repetirá una y otra vez.

Además de estas dos funciones principales, también se pueden utilizar otras funciones y bibliotecas para ampliar la funcionalidad del programa Arduino.

## Entradas y salidas

Arduino tiene una serie de pines de entrada y salida que se pueden utilizar para interactuar con el entorno. Los pines de entrada se utilizan para recibir señales de sensores u otros dispositivos, mientras que los pines de salida se utilizan para enviar señales a actuadores o para controlar otros dispositivos.

Los pines de entrada y salida se pueden configurar como digitales o analógicos. Los pines digitales tienen dos estados posibles: alto (HIGH) o bajo (LOW), mientras que los pines analógicos pueden generar y medir una amplia gama de valores.

Por ejemplo, para configurar un pin digital como salida y encender un LED conectado a ese pin, puedes usar el siguiente código:

```cpp
const int ledPin = 13;

void setup() {
  pinMode(ledPin, OUTPUT);
}

void loop() {
  digitalWrite(ledPin, HIGH);   // Encender el LED
  delay(1000);                  // Esperar 1 segundo
  digitalWrite(ledPin, LOW);    // Apagar el LED
  delay(1000);                  // Esperar 1 segundo
}
```

En este ejemplo, el pin digital 13 se configura como salida en la función `setup()`. Luego, en el bucle `loop()`, el LED se enciende y se apaga cada segundo utilizando la función `digitalWrite()`.

## Recursos adicionales

- [Sitio web oficial de Arduino](https://www.arduino.cc/): El sitio web oficial de Arduino es una excelente fuente de información y recursos, incluyendo tutoriales, documentación y una comunidad activa de usuarios.

- [Documentación de Arduino](https://www.arduino.cc/reference/en/): La documentación oficial de Arduino proporciona una referencia completa de las funciones y bibliotecas disponibles en el entorno de Arduino.

- [Arduino Forum](https://forum.arduino.cc/): El foro de Arduino es un lugar donde puedes hacer preguntas, obtener ayuda y compartir tus proyectos con la comunidad de Arduino.

- [Proyectos de Arduino en Instructables](https://www.instructables.com/circuits/arduino/projects/): Instructables es un sitio web que ofrece una amplia variedad de proyectos y tutoriales de Arduino, desde proyectos básicos hasta proyectos más avanzados.

Este repaso solo proporciona una introducción básica a Arduino. A medida que explores más proyectos y te familiarices con la plataforma, descubrirás una amplia gama

 de posibilidades y características avanzadas que te permitirán crear proyectos electrónicos interactivos y emocionantes.
