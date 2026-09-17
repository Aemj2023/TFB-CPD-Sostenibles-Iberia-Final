# Ética, privacidad y contribución a los ODS

En este documento explicamos los criterios éticos y de privacidad que hemos tenido en cuenta durante el TFB **Localización sostenible de centros de datos**.

También explicamos cómo hemos utilizado herramientas de inteligencia artificial durante el desarrollo del trabajo y la relación del proyecto con los Objetivos de Desarrollo Sostenible definidos en la Entrega 2.

## Alcance del análisis

Realizamos la comparación principal sobre 22 regiones NUTS 2 de España y Portugal. Mantenemos Andorra como una unidad complementaria cuando no dispone de información equivalente.

Con el `IIT-CPD` comparamos los territorios y analizamos distintos escenarios. No lo utilizamos para decidir una parcela concreta ni para afirmar que un territorio sea adecuado directamente para instalar un centro de datos.

Para llegar a una decisión real harían falta estudios más específicos sobre la parcela, la red eléctrica, el impacto ambiental, el urbanismo, los costes y otros condicionantes que quedan fuera del alcance del TFB.

Por eso utilizamos los rankings como una forma de comparar territorios y no como una decisión automática.

## Transparencia y calidad de los datos

En los notebooks dejamos documentadas las fuentes que hemos utilizado, las transformaciones que realizamos y las decisiones importantes que fuimos tomando durante el análisis.

No todas las fuentes corresponden al mismo año ni tienen la misma escala o cobertura. Por eso, cuando podemos, también guardamos el año y la procedencia de los datos. 

Esto es importante en fuentes como OpenStreetMap, PeeringDB o RIPE Atlas. Encontrar menos elementos registrados en un territorio no significa que exista menos infraestructura. También puede existir una diferencia en la cobertura de los datos.

Cuando podemos distinguirlo, separamos un valor igual a cero de un dato que no está disponible.

Utilizamos Isolation Forest, PCA y K-Means para entender la estructura de los datos y las diferencias entre territorios. No utilizamos estos métodos para decidir automáticamente los pesos del `IIT-CPD`.

## Privacidad y protección de la información

Trabajamos con datos territoriales, climáticos, ambientales, energéticos, socioeconómicos y de infraestructuras.

No hemos buscado ni utilizado de forma intencionada información destinada a identificar personas.

En el caso de RIPE Atlas, las posiciones de los probes ya se publican con un desplazamiento por motivos de privacidad. Nosotros utilizamos esos puntos para obtener información territorial y no intentamos averiguar su posición real.

Tampoco publicamos contraseñas, claves de API, tokens, credenciales o información confidencial.

Si utilizamos datos personales, tomamos como referencia el Reglamento (UE) 2016/679 (RGPD), sobre todo en lo relacionado con la finalidad y con utilizar únicamente los datos necesarios.

## Uso responsable de inteligencia artificial

Durante el desarrollo del TFB hemos utilizado herramientas de inteligencia artificial generativa como apoyo en algunas tareas.

Las hemos utilizado como una herramienta de ayuda y no como una fuente de datos ni como una referencia académica.

Antes de incorporar una propuesta al proyecto la revisamos y comprobamos si coincide con lo que hacen los datos, el código o la fuente correspondiente.

### Uso realizado

Las hemos utilizado para:

- organizar algunas tareas del proyecto;
- revisar fragmentos de código;
- localizar errores cuando algo no funcionaba;
- resolver dudas técnicas concretas;
- revisar si una explicación se entendía bien;
- mejorar la organización de parte de la documentación.

Las decisiones del proyecto las hemos tomado nosotros.

También hemos ejecutado los notebooks, comprobado sus resultados, revisado las variables utilizadas y validado los cambios antes de mantenerlos en la versión final.

Cuando una propuesta afecta al código, comprobamos después que funcione y que produzca el resultado esperado.

Cuando afecta a una explicación o a la documentación, comprobamos que describa lo que hemos hecho.

No utilizamos estas herramientas para sustituir la ejecución de los análisis ni nuestra interpretación de los resultados.

### Transparencia del uso

Queremos dejar claro para qué hemos utilizado estas herramientas y qué decisiones y resultados son nuestros. 

La autoría y la responsabilidad del trabajo corresponden a Antonio Eloy Martínez Jiménez y Alberto Sanz Viñuela.

No consideramos las herramientas de inteligencia artificial autoras del trabajo.

Si necesitamos explicar con más detalle su uso en la entrega final, podemos indicar qué herramienta hemos utilizado, para qué tarea la hemos usado y qué comprobación hemos realizado después.

### Verificación y límites

No utilizamos una respuesta generada por IA como evidencia científica.

Cuando necesitamos justificar un dato o una afirmación técnica acudimos a la fuente correspondiente o al resultado obtenido en nuestros notebooks.

También comprobamos los resultados numéricos con las salidas del proyecto.

No introducimos contraseñas, claves de API, tokens, datos personales innecesarios o información confidencial en estas herramientas.

También tomamos como referencia el Reglamento (UE) 2024/1689 para el uso de la inteligencia artificial y el Reglamento (UE) 2016/679 para la protección de datos. 

En cualquier caso, seguimos las normas del TFB y las indicaciones que nos dé la universidad o el tutor.

## Relación con los ODS

En la Entrega 2 relacionamos el proyecto con los **ODS 7, 9, 11 y 13**.

- **ODS 7 · Energía asequible y no contaminante:** lo relacionamos con el potencial solar, el clima y la infraestructura eléctrica.
- **ODS 9 · Industria, innovación e infraestructura:** lo relacionamos con la infraestructura eléctrica, logística y digital.
- **ODS 11 · Ciudades y comunidades sostenibles:** lo relacionamos con la cobertura del suelo, la accesibilidad y las restricciones ambientales.
- **ODS 13 · Acción por el clima:** lo relacionamos con las variables climáticas, el potencial solar y las condiciones ambientales.

Estas relaciones nos sirven para explicar qué partes del proyecto están relacionadas con cada objetivo. El `IIT-CPD` no mide directamente el cumplimiento de los ODS.

En la versión final también incorporamos el estrés hídrico. Lo consideramos una ampliación del análisis de sostenibilidad, pero mantenemos los ODS 7, 9, 11 y 13 porque son los que definimos formalmente en la Entrega 2.

## Criterios de publicación

Para mantener la trazabilidad dejamos identificadas las fuentes que utilizamos y documentamos las transformaciones realizadas.

También evitamos publicar información personal o confidencial.

Mostramos los resultados por territorios y dejamos indicadas las limitaciones que hemos encontrado en los datos y en el modelo.

Utilizamos el `IIT-CPD` para comparar territorios. Para elegir una localización concreta necesitaríamos realizar estudios técnicos específicos que no forman parte de este TFB.
