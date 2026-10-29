# A03 · Huella pública

> **Cómo usas esta plantilla**
>
> Cópiala como `README.md` en tu carpeta `A03`: en la modalidad A, `entregas/apellidoNombre/A03/`; en la modalidad B, una carpeta `A03` en tu equipo, fuera del repositorio del curso, que entregarás comprimida en el Campus Virtual. Trabaja **sobre esa copia**. No edites este archivo ni la carpeta de nadie más.
>
> Rellena los apartados sin cambiar su orden ni su numeración. Sustituye cada bloque «Qué debe contener» por tu respuesta. Si algo no te aplica, explica por qué en lugar de borrarlo. Borra estas instrucciones antes de entregar.
>
> Completa los apartados 2 y 3 **antes** de la primera consulta: en la modalidad A, haz un *commit*; en la modalidad B, anota al final del apartado 3 la fecha y hora de cierre del plan. Cada afirmación se acompaña de la fila del registro de la que sale: `(OBT-04)`, `(OBT-07, OBT-08)`.
>
> Enunciado completo: [A03 · Huella pública](https://github.com/hector-ae21/26-27-CIBINT/blob/main/actividades/A03-huella-publica/README.md)

## Estudiante

- Nombre: Sergio Rodríguez López  
- Carpeta personal: entregas/rodriguezSergio/A03/  
- Modalidad: Modalidad A · Organización  
- Objetivo: Air Europa  
- ¿Es el objetivo de tu proyecto final?: Sí.  
- Punto de partida (dominio principal o identificadores propios): aireuropa.com  
- Periodo de obtención, con zona horaria: Del 28/10/2026 al 29/10/2026 (Europe/Madrid)

---

## 1. Resumen ejecutivo

> **Qué debe contener.** Se escribe al final. Como máximo 250 palabras. Un párrafo que el destinatario pueda leer sin el resto del informe y una tabla que responda cada pregunta del apartado 2.3 con su nivel de confianza y sus referencias.

| Pregunta | Respuesta breve | Confianza | Referencias |
|---|---|---|---|
| | | | |

---

## 2. Encargo

### 2.1 Objetivo elegido

**Modalidad A.** Se ha elegido Air Europa por tratarse de la organización afectada en el caso documentado de mi proyecto final. La elección permite establecer un análisis inicial de la exposición pública de su infraestructura corporativa y canales. Antes de iniciar, se ha comprobado que existe material suficiente mediante la consulta `site:aireuropa.com filetype:pdf` en Google (realizada el 2026-10-29), obteniendo múltiples resultados de documentos públicos oficiales.

### 2.2 Requerimiento

| Componente | Contenido |
| :---- | :---- |
| Destinatario | Responsable de seguridad de la información (CISO) de Air Europa. |
| Decisión | Determinar qué elementos de la huella pública corporativa deben ser minimizados o monitorizados para prevenir escenarios de suplantación interna, fraude o recopilación de inteligencia. |
| Objeto | La huella pública digital de Air Europa, abarcando su información corporativa, canales de comunicación, documentación expuesta y relaciones institucionales. |
| Horizonte | Corto plazo (para revisión antes de finalizar el trimestre actual), sujeto a la entrega de octubre de 2026\. |
| Alcance | Dominios oficiales, perfiles corporativos en redes, información societaria y documentos corporativos (PDF) indexados. |
| Exclusiones | Queda estrictamente excluido investigar datos de clientes/empleados; analizar filtraciones; y realizar escaneos activos sobre la infraestructura. |
| Producto | Informe de huella pública estructurado, con registro de obtención, evidencias anonimizadas y recomendaciones defensivas. |

**Requerimiento en una frase:** Informe de huella pública dirigido al CISO de Air Europa para identificar y minimizar los elementos corporativos expuestos a corto plazo, excluyendo escaneos activos e investigación de datos personales.

### 2.3 Preguntas de inteligencia

| Prioridad | Pregunta | Huella que cubre | Te ayuda a decidir |
| ----: | :---- | :---- | :---- |
| 1 | ¿Qué dominios, subdominios, correos de contacto y perfiles en redes presenta u operaba Air Europa que pudieran usarse para suplantar su identidad? | De canales | Identificar canales expuestos que deban monitorizarse para prevenir campañas de *phishing* o intrusión corporativa. |
| 2 | ¿Qué información societaria, marcas registradas y filiales están accesibles en registros públicos y buscadores? | Corporativa | Evaluar si la estructura corporativa expuesta facilita ataques de suplantación interna (Fraude del CEO). |
| 3 | ¿Qué relaciones tecnológicas o correos sensibles se declaran públicamente en los sitios web o documentos indexados de la aerolínea? | De relaciones | Determinar el riesgo de exposición documental y procedimental en fuentes abiertas. |

---

## 3. Plan de obtención

### 3.1 Herramientas por pregunta

| Pregunta | Herramienta | Alternativa descartada y motivo | Entrada | Qué expone y a quién | Resultado esperado |
| :---- | :---- | :---- | :---- | :---- | :---- |
| PI-01 | Google con operadores | Búsqueda simple (genera ruido) | `site:aireuropa.com "contacto"` | Envía la consulta a Google; no interactúa con la infraestructura de Air Europa. | Redes y canales indexados. |
| PI-01 | Wayback Machine | Caché de Google | `aireuropa.com/es/vuelos` | Envía la URL al Internet Archive; no interactúa con el objetivo. | Versiones históricas de la web para comparar cambios. |
| PI-02 | OpenCorporates | BORME comercial | "Air Europa" | Envía el término a OpenCorporates; sin contacto con el objetivo. | Ficha societaria vinculada. |
| PI-03 | Google (Filetype) | Buscadores de PDFs genéricos | `site:aireuropa.com filetype:pdf` | Envía la consulta a Google; no interactúa con el objetivo. | Documentos corporativos públicos. |
| PI-03 | Intelligence X | Google simple | `aireuropa.com` | Envía el dominio a intelx.io; consulta en su archivo sin tocar al objetivo. | Subdominios y foros técnicos. |
| Todas | Maltego | Esquemas manuales en papel | Dominios y perfiles | Procesa entidades localmente y envía consultas a transformaciones OSINT autorizadas. | Grafo visual de relaciones. |

### 3.2 Herramientas que no se usan

| Herramienta | Motivo |
| :---- | :---- |
| OpenSanctions | Las preguntas se centran en la exposición técnica y societaria, no en sanciones internacionales o exposición política de personas físicas. |
| Babel Street Insights | La monitorización de menciones multilingües y seguimiento en tiempo real excede el alcance del informe. |
| Google Lens / TinEye | No se requiere verificar el origen de fotografías en este encargo, sino texto e infraestructura corporativa. |
| Hunchly | El volumen de capturas es manejable de forma manual; no se precisa archivo completo de sesión. |
| Serus | La IA asistida para buscar filtraciones de identificadores excede las exclusiones del encargo. |

### 3.3 Configuración y seguridad de la operación

Perfil de investigación dedicado en contenedor web, sin sesiones personales activas. Carpeta de trabajo aislada. Uso de correos "calcetín" para registro en herramientas obligatorias (IntelX, Maltego). No se interactúa con el objetivo bajo ninguna circunstancia.

**Modalidad B · Fecha y hora de cierre del plan:** No aplica (Modalidad A).

---

## 4. Obtención

### 4.1 Registro de obtención

> **Qué debe contener.** Una fila por consulta o acción, incluidos los errores, los resultados vacíos y las restricciones. Fecha y hora en formato `AAAA-MM-DD HH:MM`, con la zona horaria indicada en la cabecera.

| ID | Herramienta | Consulta o acción exacta | Fecha y hora | Resultado | Límite | Evidencia |
|---|---|---|---|---|---|---|
| OBT-01 | | | | | | |

### 4.2 Resultados por herramienta

> **Qué debe contener.** Para Google, Wayback Machine, la fuente societaria, Maltego y la herramienta opcional: qué pregunta respondía, qué obtuviste, con referencias, y qué límite tiene.

### 4.3 Revisión de la elección

| Pregunta | Herramienta prevista | Herramienta utilizada | Evidencia obtenida | ¿Resuelve la pregunta? | Cambio justificado |
|---|---|---|---|---|---|
| | | | | | |

---

## 5. Análisis de la huella

### 5.1 Ficha del objetivo

> **Qué debe contener.** Es el punto de partida de la A04. Una fila por campo:
>
> - modalidad A: nombre legal, marcas, filiales o entidades relacionadas, dominios oficiales, canales y perfiles oficiales, proveedores observados;
> - modalidad B: nombre y alias, cuentas y perfiles, correos públicos, relaciones profesionales o académicas, webs y dominios, documentos publicados.

| Campo | Dato | Referencia | Fecha del dato | Precaución |
|---|---|---|---|---|
| | | | | |

### 5.2 Huella por dimensiones

> **Qué debe contener.** Para cada huella, dos partes separadas: **Observado**, con referencias, y **Valoración**, con fiabilidad de la fuente, credibilidad de la información y lo que falta.

#### Corporativa o profesional

#### De canales

#### De relaciones

### 5.3 Grafo de relaciones

> **Qué debe contener.** La imagen del grafo exportado desde Maltego, enlazada desde `evidencias/`, y una leyenda que distinga relaciones observadas, declaradas y pendientes, cada una con su referencia.

| Relación | Tipo | Referencia |
|---|---|---|
| | | |

### 5.4 Valoración de hallazgos clave

| Hallazgo | Referencias | Fiabilidad de la fuente | Credibilidad de la información | Hecho o inferencia | Contraste independiente |
|---|---|---|---|---|---|
| | | | | | |

---

## 6. Perspectiva del atacante

> **Qué debe contener.** Al menos tres filas, cada una a partir de un hallazgo propio. Describe el riesgo sin instrucciones operativas.

| Información visible | Referencia | Cómo podría aprovecharla un atacante | A qué afectaría | Medida defensiva | Prioridad |
|---|---|---|---|---|---|
| | | | | | |

---

## 7. Limitaciones, datos descartados e incidencias

> **Qué debe contener.** Preguntas que no has podido responder y por qué. Datos que has descartado por quedar fuera del alcance, incluidos los homónimos y los datos de terceros. Incidencias, solo con su categoría y su fila `OBT`, e indicación de si avisaste por el canal privado. Si no hubo incidencias, escríbelo.

---

## 8. Índice de evidencias

| Evidencia | Qué muestra | Fila del registro | Qué se ha ocultado |
|---|---|---|---|
| | | | |

---

## 9. Uso de inteligencia artificial

Ver [registro-ia.md](registro-ia.md).

---

## Comprobación

- [ ] El objetivo cumple los requisitos de mi modalidad y no investigo a ninguna otra persona.
- [ ] Cerré los apartados 2 y 3 antes de la obtención: *commit* en la modalidad A, fecha de cierre en la modalidad B.
- [ ] Cada afirmación lleva su referencia `OBT` y la he comprobado.
- [ ] Las capturas están recortadas y anonimizadas.
- [ ] Entrego antes del viernes 30 de octubre a las 23:59.
- [ ] Modalidad A: solo he modificado `entregas/apellidoNombre/A03/`. Modalidad B: nada está en el repositorio del curso.
