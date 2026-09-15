# Ética, privacidad y contribución a los ODS

Este documento resume los criterios éticos, de privacidad y de uso responsable de inteligencia artificial aplicados en el TFB **Localización sostenible de centros de datos**.

También recoge la relación del proyecto con los Objetivos de Desarrollo Sostenible definidos en la Entrega 2.

## Alcance del análisis

La comparación principal se realiza sobre 22 regiones NUTS 2 de España y Portugal. Andorra se mantiene como unidad complementaria cuando no dispone de información equivalente.

El `IIT-CPD` permite comparar territorios y estudiar distintos escenarios de decisión. No selecciona una parcela concreta ni sustituye los estudios técnicos, ambientales, urbanísticos, energéticos o económicos necesarios para una implantación real.

Por este motivo, los rankings se utilizan como apoyo a la decisión y no como una recomendación automática.

## Transparencia y calidad de los datos

Los notebooks documentan las fuentes utilizadas, las principales transformaciones y las decisiones tomadas durante el análisis.

Isolation Forest, PCA y K-Means ayudan a estudiar la estructura de los datos, pero no asignan automáticamente los pesos del `IIT-CPD`.

Las fuentes tampoco presentan siempre la misma fecha, escala o cobertura. Esto es especialmente importante en OpenStreetMap, PeeringDB y RIPE Atlas, donde una menor presencia de elementos registrados no significa necesariamente que exista menos infraestructura real.

Cuando la información disponible lo permite diferenciamos entre un valor igual a cero, un dato no disponible y una posible falta de cobertura.

## Privacidad y protección de la información

El proyecto utiliza principalmente información territorial, climática, ambiental, energética, socioeconómica y de infraestructuras.

No trabajamos de forma intencionada con datos destinados a identificar personas.

RIPE Atlas publica las posiciones de sus probes con un desplazamiento deliberado por motivos de privacidad. En nuestro análisis utilizamos estos puntos para generar indicadores territoriales y no intentamos reconstruir sus ubicaciones exactas.

Tampoco publicamos contraseñas, claves de API, tokens, credenciales, datos personales o información confidencial.

Cuando pudiera existir tratamiento de datos personales tomamos como referencia los principios establecidos en el Reglamento (UE) 2016/679 (RGPD), especialmente la transparencia, la limitación de la finalidad y la minimización de los datos.

## Uso responsable de inteligencia artificial

Durante el desarrollo del TFB hemos utilizado herramientas de inteligencia artificial generativa como apoyo en determinadas tareas del proceso de trabajo.

Su utilización se ha realizado siguiendo criterios de transparencia, revisión humana y responsabilidad de los autores. La IA no se considera una fuente de datos ni una referencia académica, y sus respuestas no se incorporan al proyecto sin revisión.

### Uso realizado

Las herramientas de IA se han utilizado principalmente para:

- apoyo en la planificación y organización de tareas;
- revisión y mejora de fragmentos de código;
- ayuda en la identificación y depuración de errores;
- asistencia puntual en cuestiones técnicas;
- revisión de claridad, estructura y documentación del proyecto.

Las fuentes de datos, la ejecución de los notebooks, la selección final de variables y métodos, la comprobación de los resultados y las decisiones que forman parte del TFB permanecen bajo responsabilidad de los autores.

Cuando una propuesta obtenida mediante IA afecta al código o a la documentación, la revisamos antes de incorporarla y la contrastamos con la ejecución real del proyecto o con la fuente correspondiente.

### Transparencia del uso

Siguiendo prácticas que actualmente aplican distintas universidades en trabajos académicos, consideramos importante declarar:

1. la herramienta utilizada;
2. la finalidad para la que se utilizó;
3. el tipo de tarea en la que intervino;
4. el grado aproximado de asistencia;
5. la revisión realizada posteriormente por los autores.

Cuando sea necesario en la entrega final, esta información puede ampliarse mediante una declaración o anexo específico de uso de inteligencia artificial.

No atribuimos autoría a las herramientas de IA. La autoría, la revisión y la responsabilidad académica del trabajo corresponden a Antonio Eloy Martínez Jiménez y Alberto Sanz Viñuela.

### Verificación y límites

No utilizamos una respuesta generada por IA como evidencia científica ni como sustituto de una fuente original.

Los datos, referencias, resultados numéricos y afirmaciones técnicas relevantes se comprueban mediante las fuentes empleadas en el proyecto o mediante la ejecución de los notebooks.

Tampoco introducimos deliberadamente en estas herramientas contraseñas, claves de API, tokens, datos personales innecesarios o información confidencial.

Como referencia general de uso responsable tenemos en cuenta los principios de alfabetización en inteligencia artificial del Reglamento (UE) 2024/1689 y, cuando pudiera existir tratamiento de información personal, los principios de protección de datos del Reglamento (UE) 2016/679.

Estas referencias no sustituyen la normativa académica aplicable al TFB. En caso de existir instrucciones específicas de la universidad, de la titulación o del tutor sobre el uso de inteligencia artificial, estas tienen prioridad.

## Relación con los ODS

La Entrega 2 relacionó el proyecto con los **ODS 7, 9, 11 y 13**.

- **ODS 7 · Energía asequible y no contaminante:** potencial solar, clima e infraestructura eléctrica.
- **ODS 9 · Industria, innovación e infraestructura:** infraestructura eléctrica, logística y digital.
- **ODS 11 · Ciudades y comunidades sostenibles:** cobertura del suelo, accesibilidad y restricciones ambientales.
- **ODS 13 · Acción por el clima:** variables climáticas, potencial solar y condiciones ambientales.

Estas relaciones indican qué partes del proyecto tienen relación con esos objetivos, pero el `IIT-CPD` no mide directamente su cumplimiento.

La versión final incorpora además una dimensión de estrés hídrico. La consideramos una ampliación del análisis de sostenibilidad, pero mantenemos los ODS 7, 9, 11 y 13 como los definidos formalmente en la Entrega 2.

## Criterios de publicación

Para mantener la trazabilidad del proyecto conservamos la atribución de las fuentes, documentamos las principales transformaciones y evitamos publicar información personal o confidencial.

Los resultados se presentan principalmente de forma territorial y agregada, y mantenemos visibles las limitaciones de los datos y del modelo.

El `IIT-CPD` es una herramienta de comparación territorial. La elección definitiva de una localización requeriría estudios técnicos específicos.
