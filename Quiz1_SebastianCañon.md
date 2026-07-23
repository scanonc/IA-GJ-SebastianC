# Actividad de Clase: Analizando Agentes de IA con Hugging Face Spaces

## Objetivo

Explorar aplicaciones reales de Inteligencia Artificial en **Hugging
Face Spaces** y analizarlas desde la perspectiva de los **agentes
racionales**.

Al finalizar la actividad, los estudiantes deberán ser capaces de:

-   Identificar los componentes **PEAS** de un agente.
-   Clasificar las propiedades del entorno.
-   Proponer qué tipo de programa de agente podría implementarse detrás
    del sistema.
-   Justificar sus respuestas.

------------------------------------------------------------------------

## Instrucciones

1.  Ingresen a **https://huggingface.co/spaces**.
2.  Exploren diferentes Spaces.
3.  Seleccionen uno que les parezca interesante.
4.  Interactúen con el sistema durante algunos minutos.
5.  Completen la siguiente ficha de análisis.

------------------------------------------------------------------------

# Ficha de análisis

## 1. Nombre del Space

**Nombre:** Dream Motion Pro

**Enlace:** https://huggingface.co/spaces/dream2589632147/Dream-wan2-2-fp8da-aoti-preview-2

------------------------------------------------------------------------

## 2. ¿Qué hace el agente?

Describa en dos o tres líneas cuál es la función del sistema.

El agente recibe una imagen y en base a ella crea un video que continua de forma coherente
con la secuencia de la imagen.

------------------------------------------------------------------------

## 3. Análisis PEAS

  Elemento          Respuesta
  ----------------- ----------------------------------------------------
  **Performance**   Que el video sea fluido, realista y coherente con la imagen que ingreso el usuario.
  **Environment**   Imagenes que el usuario le proporcione.
  **Actuators**     Construye un video basado en una imagen proporcionada por el usuario.
  **Sensors**       Imagen y promt proporcionado por el usuario, parametros de video

------------------------------------------------------------------------

## 4. Clasificación del entorno

Complete la siguiente tabla y justifique brevemente cada respuesta.

  Propiedad      Clasificación     Justificación
  -------------- ----------------- ---------------
  Observable     Parcial           El agente solo conoce la imagen y la información que el usuario ingresa.
  Determinista   No                No porque se puede ingresar la misma imagen y el agente genera videos diferentes.
  Episódico      Sí                Si porque cada video que se genera es independiente o no tiene que ver con los anteriores generados.
  Estático       Sí                Si porque la imagen de entrada no cambia despues de que el agente actue, no cambia el entorno.
  Discreto       No                Trabaja con imagenes y videos que son información continua.
  Conocido       Sí                El agente conoce como procesar las entradas y generar el video segun el modelo con el que fue entrenado.

------------------------------------------------------------------------

## 5. ¿Qué tipo de programa de agente creen que es?

Seleccione la opción que consideren más adecuada y explique por qué.

-   Agente de reflejo simple
-   Agente basado en modelo
-   Agente basado en objetivos
-   Agente basado en utilidad
-   Agente con aprendizaje

Yo diria que la opcion mas adecuada es de aprendizaje porque estos agentes de generacion de videos son entrenados con
con grandes cantidades de imagenes y videos para aprender los patrones de movimiento, con ese aprendizaje pueden generar
nuevas secuencias a partir de imagenes que no han visto antes.


------------------------------------------------------------------------

# Discusión en clase

Después de las presentaciones, discutiremos preguntas como:

-   ¿Dos Spaces diferentes pueden compartir el mismo tipo de entorno?
-   ¿Es posible saber con certeza qué tipo de agente implementa un Space
    únicamente observándolo?
-   ¿Qué diferencia existe entre el comportamiento observable de un
    agente y su implementación interna?

------------------------------------------------------------------------

# Reto adicional

Encuentre un Space que pueda clasificarse como:

1.  **Totalmente observable, determinista y episódico.**
2.  **Parcialmente observable, estocástico y secuencial.**

Justifique su respuesta.

------------------------------------------------------------------------

# Rúbrica (10 puntos)

| Criterio | Puntos |
|-----------|:------:|
| Descripción correcta del Space | 2 |
| Identificación de PEAS | 3 |
| Clasificación del entorno | 3 |
| Justificación del tipo de agente | 2 |
| **Total** | **10** |

------------------------------------------------------------------------