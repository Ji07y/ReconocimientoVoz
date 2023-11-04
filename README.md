# Reconocimiento de Voz en Unity
![Captura de pantalla 2023-11-03 224513](https://github.com/Ji07y/ReconocimientoVoz/assets/85076732/a6196efe-17c5-4ece-b560-c71a7def2f9f)
https://youtu.be/2DlCYvUwNsU

Este es un proyecto de muestra que demuestra cómo usar el reconocimiento de voz en Unity para controlar un objeto en el juego. En este caso, hemos creado un escenario simple en el que puedes activar y desactivar un objeto llamado "arma" utilizando comandos de voz.

## Requisitos

Antes de ejecutar este proyecto, asegúrate de tener instalado lo siguiente:

- Unity 3D 
- Micrófono (para la entrada de voz)

## Cómo Funciona

Este proyecto se basa en el reconocimiento de voz. Cuando se ejecuta el juego, el objeto "arma" está desactivado por defecto. Luego, hemos configurado palabras clave como "activar arma" y "desactivar arma" que, cuando se pronuncian, activan o desactivan el objeto "arma" en el juego.

## Configuración

- Asegúrate de tener Unity instalado en tu sistema.
- Abre el proyecto en Unity.
- Asegúrate de tener un objeto llamado "arma" en la jerarquía.
- Configura el reconocimiento de voz con las palabras clave y las funciones correspondientes en el script.

## Ejecución

- Ejecuta el proyecto en Unity.
- Activa el micrófono y pronuncia "activar arma" para ver cómo el objeto "arma" se activa.
- Pronuncia "desactivar arma" para ocultar el objeto nuevamente.

## Código Fuente
![image](https://github.com/Ji07y/ReconocimientoVoz/assets/85076732/9cf14b1e-f190-4e5f-963a-2dacb886c675)


El código fuente se encuentra en el archivo .cs proporcionado, y aquí se presenta una explicación de las partes clave:

- **KeywordRecognizer**: Inicializamos un objeto `KeywordRecognizer` que nos permite reconocer palabras clave en comandos de voz.

- **Dictionary**: Creamos un diccionario `wordToAction` que mapea palabras clave a acciones. En este ejemplo, configuramos "activar arma" para invocar la función `ActivarArma()` y "desactivar arma" para invocar la función `DesactivarArma()`.

- **Start()**: En el método `Start()`, desactivamos inicialmente el objeto "arma" para que esté oculto cuando el juego comienza.

- **KeywordRecognizer Configuration**: Configuramos el `KeywordRecognizer` con las palabras clave definidas en el diccionario. Cuando se pronuncian estas palabras clave, el reconocimiento de voz dispara el evento `OnPhraseRecognized`.

- **WordRecognized()**: Este método se ejecuta cuando se reconoce una palabra clave. Registra la palabra detectada en la consola y luego invoca la función asociada en el diccionario, lo que activa o desactiva el objeto "arma".

- **Funciones ActivarArma() y DesactivarArma()**: Estas funciones se utilizan para cambiar el estado del objeto "arma", activándolo o desactivándolo según corresponda.

## Uso

Al ejecutar el juego, el micrófono se activa y se puede pronunciar "activar arma" para hacer que el objeto "arma" aparezca y "desactivar arma" para ocultarlo nuevamente. Esto agrega una interacción adicional a tus proyectos de Unity al permitir el control por voz.

¡Diviértete jugando con el reconocimiento de voz en Unity!
