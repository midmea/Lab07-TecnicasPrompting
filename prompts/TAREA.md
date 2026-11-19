# Tarea: Mi prompt avanzado 
Como evitar caer en uso negativo de IA en procesos de aprendizaje de TI
 
## Tarea elegida 
Generar casos de prueba para el formulario de registro de usuarios de una aplicación web (nombre, correo, contraseña y confirmar contraseña). Elegí esta tarea porque en desarrollo de software las pruebas deben cubrir no solo los casos normales, sino también los casos límite, y es una tarea que se repite en cualquier proyecto.
 
## Version 1: prompt basico 

Dame casos de prueba para un registro de usuarios.
 
## Version 2 

<rol>Actúa como analista de pruebas de software (QA) con experiencia en aplicaciones web, que escribe casos de prueba para un equipo de desarrollo junior.</rol>
 
<contexto>Formulario de registro de una aplicación web con los campos: nombre completo, correo electrónico, contraseña y confirmar contraseña. Reglas: la contraseña debe tener entre 8 y 20 caracteres, al menos una mayúscula y un número; el correo no puede estar registrado previamente.</contexto>
 
<tarea>Escribe 8 casos de prueba para este formulario.</tarea>
 
<formato>Tabla con las columnas: ID, escenario, datos de entrada, resultado esperado.</formato>

 
## Version 3: prompt final 

<rol>Actúa como analista de pruebas de software (QA) con experiencia en aplicaciones web, que escribe casos de prueba para un equipo de desarrollo junior.</rol>
 
<contexto>Formulario de registro de una aplicación web con los campos: nombre completo, correo electrónico, contraseña y confirmar contraseña. Reglas: la contraseña debe tener entre 8 y 20 caracteres, al menos una mayúscula y un número; el correo no puede estar registrado previamente.</contexto>
 
<tarea>
Piensa paso a paso:
1. Identifica cada campo y sus reglas de validación.
2. Para cada campo, determina los valores válidos, los inválidos y los valores límite.
3. Con ese análisis, escribe 10 casos de prueba que cubran casos positivos, negativos y límite.
Después de la tabla, revisa tu propio trabajo: ¿faltan casos límite como campos vacíos, correo sin @, contraseña de 7 o de 21 caracteres, contraseñas que no coinciden o espacios en blanco? Agrega los que falten e indica cuáles agregaste.
</tarea>
 
<ejemplos>
| ID | Escenario | Datos de entrada | Resultado esperado |
| RU-01 | Registro exitoso con datos válidos | Nombre: Ana Pérez; Correo: ana@mail.com; Contraseña: Clave1234; Confirmar: Clave1234 | Cuenta creada y mensaje de confirmación |
| RU-02 | Correo sin arroba | Nombre: Ana Pérez; Correo: anamail.com; Contraseña: Clave1234; Confirmar: Clave1234 | Mensaje de error: "Correo no válido" |
</ejemplos>
 
<formato>
Responde en español, en este orden:
1. Resumen del análisis (máximo 5 líneas).
2. Tabla con las columnas ID, escenario, datos de entrada y resultado esperado, siguiendo el formato de los ejemplos (IDs RU-01, RU-02, ...).
3. Sección "Casos agregados en la revisión".
</formato>

 
## Tecnicas usadas en el prompt final 
 role prompting
 chain of thought
 few-shot
 prompt estructurado

## Evaluacion del resultado 
 
## Por que elegi estas tecnicas 
Porque nesecitaba que tenga un rol y punto de vista del analista 