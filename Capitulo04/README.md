# Elaboración del Brief de Innovación en Word y Automatización de la Presentación Ejecutiva del Plan de Lanzamiento en PowerPoint

## Metadatos

| Campo | Detalle |
|---|---|
| **Duración** | 72 minutos |
| **Complejidad** | Alta |
| **Nivel Bloom** | Crear |
| **Módulo** | 4 — Integración End-to-End y Entregables Ejecutivos |
| **Caso de negocio** | Marca Nexo — Línea de bebidas funcionales |

---

## Descripción General

Este laboratorio es el cierre integrador del curso. Consolidarás todos los outputs generados en los módulos anteriores (informe de posicionamiento M1, estrategia comercial y precios M2, kit de comunicación M3) en un paquete ejecutivo completo listo para presentar a la dirección. Trabajarás en secuencia lógica a través de cuatro herramientas de Microsoft 365 — Word, PowerPoint, Outlook y Teams — utilizando Copilot como motor de automatización en cada etapa. Al finalizar, dispondrás de un portafolio profesional de cinco entregables (M1 a M4) que demuestra dominio end-to-end de Microsoft 365 Copilot aplicado a comunicación y estrategia comercial.

---

## Objetivos de Aprendizaje

Al completar este laboratorio serás capaz de:

- [ ] Redactar un Brief de Innovación completo y estructurado en Word con Copilot, integrando como insumos los outputs de los tres módulos anteriores (posicionamiento, estrategia comercial y kit de comunicación).
- [ ] Automatizar la creación de una Presentación Ejecutiva de plan de lanzamiento en PowerPoint con Copilot, transformando el Brief de Innovación en diapositivas con narrativa ejecutiva y visualizaciones.
- [ ] Aplicar Copilot en Outlook para redactar comunicaciones diferenciadas por audiencia (equipo directivo interno y distribuidores externos).
- [ ] Utilizar Copilot en Teams para preparar el resumen de una reunión de kickoff, generando acuerdos, próximos pasos y asignación de responsables de forma automatizada.
- [ ] Aplicar ingeniería de prompts avanzada con el modelo ACRA y la jerarquía de mensajes aprendidos en la lección 4.1 para enriquecer los entregables finales.

---

## Prerrequisitos

### Conocimientos Previos

| Requisito | Detalle |
|---|---|
| Módulos 1, 2 y 3 completados | Los archivos canónicos de cada módulo deben estar finalizados y guardados en OneDrive |
| Jerarquía de mensajes | Comprensión de los 3 niveles (primario, secundario, soporte) cubiertos en la lección 4.1 |
| Modelo ACRA | Capacidad de aplicar Aceptar-Clarificar-Responder-Avanzar para manejo de objeciones |
| Estructura de presentaciones ejecutivas | Familiaridad con flujo: problema → solución → plan → KPIs |
| Ingeniería de prompts | Experiencia con prompts contextualizados en Word, Excel y PowerPoint de módulos previos |

### Acceso y Licencias

| Requisito | Verificación |
|---|---|
| Licencia **Microsoft Copilot for Microsoft 365** activa | Abrir Word → verificar icono de Copilot en la cinta de opciones |
| Cuenta corporativa con buzón de Outlook operativo | Enviar un correo de prueba a uno mismo |
| Microsoft Teams (New Teams) con sesión iniciada | Verificar acceso al chat de Copilot dentro de Teams |
| OneDrive sincronizado | Confirmar que la carpeta `Documentos/CopilotComunicacionEstrategia/` es accesible |

### Archivos Requeridos

Los siguientes archivos deben existir en OneDrive **antes** de iniciar:

| Archivo | Ruta en OneDrive | Origen |
|---|---|---|
| `M1_Informe_Ejecutivo_Posicionamiento.docx` | `Documentos/CopilotComunicacionEstrategia/M1_Informe_Ejecutivo/` | Módulo 1 |
| `M2_Estrategia_Comercial_Precios.xlsx` | `Documentos/CopilotComunicacionEstrategia/M2_Estrategia_Comercial/` | Módulo 2 |
| `M3_Kit_Comunicacion_Distribuidores.docx` | `Documentos/CopilotComunicacionEstrategia/M3_Kit_Comunicacion/` | Módulo 3 |

> **⚠️ Nota:** Si no completaste algún módulo anterior, solicita al instructor los **archivos semilla** correspondientes antes de continuar.

---

## Entorno de Laboratorio

### Hardware Mínimo

| Componente | Especificación |
|---|---|
| Procesador | Intel Core i5 8ª gen. / AMD Ryzen 5 3000 o superior |
| RAM | 16 GB recomendado (mínimo 8 GB) |
| Pantalla | 1920×1080 recomendado (mínimo 1366×768) |
| Almacenamiento libre | 10 GB (SSD recomendado) |
| Red | Descarga ≥ 10 Mbps / Subida ≥ 5 Mbps |
| Periféricos | Ratón externo, cámara web, micrófono, auriculares |

### Software Requerido

| Aplicación | Versión Mínima |
|---|---|
| Microsoft 365 Apps (Word, PowerPoint, Outlook) | 2405 (Build 17628.20144) — Canal Mensual |
| Microsoft Teams (New Teams) | 24046.2813.2908.4068 |
| OneDrive for Business | 24.071.0407.0003 |
| Microsoft Edge | 126.0.2592.68 |

### Configuración Inicial del Entorno

Antes de comenzar, ejecuta estas verificaciones:

1. Abre **Explorador de archivos** → navega a `OneDrive - [Tu Organización]/Documentos/CopilotComunicacionEstrategia/`.
2. Verifica que existan las subcarpetas `M1_Informe_Ejecutivo/`, `M2_Estrategia_Comercial/`, `M3_Kit_Comunicacion/`.
3. Crea la subcarpeta del módulo actual si no existe:

```
M4_Brief_Presentacion/
```

4. Confirma que los tres archivos previos (M1, M2, M3) muestran el ícono de **nube con check verde** en OneDrive (sincronizados).
5. Abre **Word** → haz clic en el icono de **Copilot** en la cinta → confirma que el panel lateral se abre correctamente.
6. Repite la verificación de Copilot en **PowerPoint** y **Outlook**.

---

## Instrucciones Paso a Paso

---

### PARTE 1 — Brief de Innovación en Word (25 minutos)

---

#### Paso 1: Crear el documento y establecer el contexto inicial con Copilot

**Objetivo:** Crear el archivo `M4_Brief_Innovacion.docx` y utilizar Copilot para generar la estructura completa del brief referenciando los archivos de módulos anteriores.

**Instrucciones:**

1. Abre **Microsoft Word** y selecciona **Documento en blanco**.

2. Guarda inmediatamente el archivo:
   - **Archivo** → **Guardar como** → **OneDrive** → navega a `Documentos/CopilotComunicacionEstrategia/M4_Brief_Presentacion/`.
   - Nombre del archivo: `M4_Brief_Innovacion.docx`
   - Haz clic en **Guardar**.

3. Espera 5 segundos a que OneDrive confirme la sincronización (ícono de nube con check en la barra de título).

4. Haz clic en el icono de **Copilot** en la cinta de opciones (pestaña **Inicio**) para abrir el panel lateral de Copilot.

5. En el panel de Copilot, escribe el siguiente prompt fundacional. **Antes de enviarlo**, utiliza el botón de **adjuntar archivo** (ícono de clip o "/") para referenciar los tres archivos previos:

```text
Redacta un Brief de Innovación ejecutivo para el lanzamiento de una nueva 
bebida funcional de la marca Nexo (línea de bebidas con electrolitos, 
sin azúcar añadida, posicionada en "rendimiento accesible para todos").

Usa como insumos los siguientes documentos que adjunto:
- /M1_Informe_Ejecutivo_Posicionamiento.docx (contexto competitivo y posicionamiento)
- /M2_Estrategia_Comercial_Precios.xlsx (estrategia de canales y modelo de precios)
- /M3_Kit_Comunicacion_Distribuidores.docx (mensajes clave y comunicación por audiencia)

Estructura el brief con las siguientes 8 secciones, cada una con su 
encabezado de nivel 2:
1. Resumen del Contexto Competitivo
2. Oportunidad de Mercado Identificada
3. Descripción del Concepto de Innovación
4. Estrategia de Canales y Precios Propuesta
5. Mensajes Clave y Propuesta de Comunicación
6. Objetivos de Negocio y KPIs del Lanzamiento
7. Recursos Requeridos y Cronograma de Alto Nivel
8. Criterios de Éxito y Métricas de Seguimiento

Tono: ejecutivo, directo, orientado a decisiones. 
Extensión: 1,500-2,000 palabras totales.
Incluye una tabla resumen de KPIs en la sección 6 y un cronograma 
tipo Gantt simplificado (tabla) en la sección 7.
```

6. Para referenciar cada archivo, escribe `/` en el campo de prompt y selecciona el archivo correspondiente de la lista de archivos recientes de OneDrive. Si no aparece, navega manualmente seleccionando **Archivos** en el menú desplegable.

7. Presiona **Enter** o haz clic en **Enviar** para ejecutar el prompt.

8. Espera a que Copilot genere el contenido completo (puede tardar 15-30 segundos).

**Resultado Esperado:**

Copilot insertará en el documento un brief estructurado con las 8 secciones solicitadas. El contenido debe:
- Referenciar datos específicos del informe de posicionamiento (M1) en la sección 1.
- Incluir elementos de la estrategia de precios (M2) en la sección 4.
- Incorporar mensajes clave del kit de comunicación (M3) en la sección 5.
- Contener una tabla de KPIs y un cronograma simplificado.

**Verificación:**

- [ ] El documento contiene exactamente 8 secciones con encabezados de Nivel 2.
- [ ] Las secciones 1, 4 y 5 contienen referencias reconocibles a los archivos M1, M2 y M3 respectivamente.
- [ ] Existe al menos una tabla en la sección 6 (KPIs) y otra en la sección 7 (cronograma).
- [ ] El tono es ejecutivo y la extensión aproximada es 1,500-2,000 palabras.

---

#### Paso 2: Enriquecer el brief con jerarquía de mensajes y modelo ACRA

**Objetivo:** Integrar los conceptos de jerarquía de mensajes para punto de venta y el modelo ACRA de manejo de objeciones como secciones complementarias del brief, aplicando lo aprendido en la lección 4.1.

**Instrucciones:**

1. Posiciona el cursor al final de la **Sección 5 (Mensajes Clave y Propuesta de Comunicación)**.

2. En el panel de Copilot, escribe el siguiente prompt:

```text
Dentro de la sección "Mensajes Clave y Propuesta de Comunicación" de este 
documento, agrega una subsección titulada "Jerarquía de Mensajes para 
Punto de Venta" con la siguiente estructura:

- Nivel 1 (Mensaje primario, máx. 6 palabras): para exhibidor de piso 
  y stopper de anaquel.
- Nivel 2 (Mensaje secundario, máx. 20 palabras): para cenefa de anaquel 
  y panel lateral de exhibidor.
- Nivel 3 (Mensaje de soporte, máx. 40 palabras): para folleto del 
  promotor y ficha técnica.

Contexto: 
- Territorio de marca: "rendimiento accesible para todos"
- Beneficio rector: "hidratación con electrolitos sin azúcar añadida"
- Shopper: adulto 28-40 años, compra en supermercado, desconfía de 
  productos "saludables" por precio

Incluye una variante de cada nivel para promoción de lanzamiento.
Presenta todo en formato de tabla.
```

3. Presiona **Enter** y espera la generación.

4. Revisa que la tabla generada contenga los 3 niveles con sus variantes. Si algún mensaje excede el límite de palabras, selecciónalo y pide a Copilot: `Acorta este mensaje a máximo [6/20/40] palabras manteniendo el impacto.`

5. Ahora posiciona el cursor al final de la **Sección 5** (después de la tabla de jerarquía recién creada).

6. Escribe el siguiente prompt para agregar el argumentario ACRA:

```text
Agrega una subsección titulada "Argumentario de Manejo de Objeciones 
(Modelo ACRA)" después de la jerarquía de mensajes.

Genera respuestas ACRA (Aceptar, Clarificar, Responder, Avanzar) para 
las 3 objeciones más frecuentes en el lanzamiento de Marca Nexo:

1. "Es muy caro comparado con las bebidas deportivas existentes."
2. "Ya tenemos demasiadas opciones de bebidas funcionales en el anaquel."
3. "Nadie conoce la marca Nexo, no va a rotar."

Para cada objeción genera DOS versiones:
a) Versión para el gerente de categoría del supermercado (enfocada en 
   margen, rotación y diferenciación de anaquel).
b) Versión para el promotor en piso de venta dirigida al consumidor 
   final (enfocada en valor percibido y beneficio personal).

Tono conversacional, máximo 80 palabras por respuesta ACRA completa.
Formato: tabla con columnas [Objeción | Audiencia | Aceptar | Clarificar | Responder | Avanzar].
```

7. Presiona **Enter** y espera la generación.

8. Guarda el documento: **Ctrl + S**.

**Resultado Esperado:**

La sección 5 del brief ahora contiene:
- Una subsección con tabla de jerarquía de mensajes (3 niveles × 2 variantes = 6 mensajes).
- Una subsección con tabla ACRA (3 objeciones × 2 audiencias = 6 filas de argumentarios).

**Verificación:**

- [ ] La tabla de jerarquía tiene 3 niveles con mensajes dentro de los límites de palabras especificados.
- [ ] La tabla ACRA contiene 6 filas (3 objeciones × 2 versiones por audiencia).
- [ ] Cada respuesta ACRA tiene los 4 componentes (Aceptar, Clarificar, Responder, Avanzar).
- [ ] El tono de las versiones para gerente de categoría difiere claramente del tono para consumidor final.

---

#### Paso 3: Revisar, refinar y finalizar el Brief de Innovación

**Objetivo:** Utilizar Copilot para realizar una revisión de calidad del documento completo, asegurar coherencia narrativa y aplicar formato profesional.

**Instrucciones:**

1. Con el documento completo visible, abre el panel de Copilot y escribe:

```text
Revisa este documento completo y evalúa:
1. ¿Las 8 secciones mantienen coherencia narrativa entre sí?
2. ¿El tono es consistentemente ejecutivo en todo el documento?
3. ¿Hay redundancias o contradicciones entre secciones?
4. ¿Los KPIs de la sección 6 son medibles y tienen plazo definido?
5. ¿El cronograma de la sección 7 es realista para un lanzamiento 
   de bebida funcional?

Proporciona un resumen de hallazgos y sugiere 3 mejoras concretas.
```

2. Presiona **Enter** y revisa los hallazgos de Copilot.

3. Aplica las mejoras sugeridas que consideres pertinentes. Para cada mejora, puedes seleccionar el texto a modificar y usar Copilot con un prompt específico como:

```text
Reescribe este párrafo incorporando [la mejora específica sugerida], 
manteniendo el tono ejecutivo y la extensión similar.
```

4. Agrega una **portada** al documento:
   - Ve a **Insertar** → **Portada** → selecciona un diseño profesional.
   - Completa los campos: **Título:** "Brief de Innovación — Marca Nexo: Línea de Bebidas Funcionales", **Subtítulo:** "Plan de Lanzamiento — [Mes y Año]", **Autor:** [Tu nombre].

5. Agrega una **tabla de contenido** automática:
   - Posiciona el cursor después de la portada.
   - Ve a **Referencias** → **Tabla de contenido** → selecciona un formato automático.

6. Guarda el documento final: **Ctrl + S**.

7. Verifica que el archivo esté sincronizado en OneDrive (ícono de nube con check verde).

**Resultado Esperado:**

Un documento Word profesional de 8-12 páginas con portada, tabla de contenido, 8 secciones estructuradas, tablas de KPIs, cronograma, jerarquía de mensajes y argumentario ACRA.

**Verificación:**

- [ ] El documento tiene portada profesional con título, subtítulo y autor.
- [ ] La tabla de contenido refleja las 8 secciones y subsecciones.
- [ ] El documento está guardado como `M4_Brief_Innovacion.docx` en la ruta correcta de OneDrive.
- [ ] Copilot no identificó contradicciones críticas entre secciones.

---

### PARTE 2 — Presentación Ejecutiva en PowerPoint (30 minutos)

---

#### Paso 4: Generar la presentación automáticamente desde el Brief de Innovación

**Objetivo:** Utilizar la función de Copilot en PowerPoint para crear automáticamente una presentación ejecutiva de 10-15 diapositivas a partir del Brief de Innovación.

**Instrucciones:**

1. Abre **Microsoft PowerPoint**.

2. En la pantalla de inicio, selecciona **Presentación en blanco**.

3. Antes de hacer cualquier otra cosa, guarda el archivo:
   - **Archivo** → **Guardar como** → **OneDrive** → `Documentos/CopilotComunicacionEstrategia/M4_Brief_Presentacion/`
   - Nombre: `M4_Presentacion_Ejecutiva_Lanzamiento.pptx`
   - Haz clic en **Guardar**.

4. Haz clic en el icono de **Copilot** en la cinta de opciones de PowerPoint.

5. En el panel de Copilot, selecciona la opción **"Crear presentación a partir de archivo"** (o escribe el prompt a continuación si la opción directa no aparece).

6. Utiliza el botón de adjuntar archivo (`/`) para referenciar el Brief de Innovación y escribe el siguiente prompt:

```text
Crea una presentación ejecutiva de 12-15 diapositivas a partir del archivo 
/M4_Brief_Innovacion.docx para presentar el plan de lanzamiento de 
Marca Nexo (bebidas funcionales) ante el comité directivo.

Estructura requerida:
1. Portada (nombre del proyecto, fecha, equipo)
2. Agenda
3. Contexto competitivo (resumen de hallazgos clave)
4. Oportunidad de mercado (tamaño, tendencia, gap)
5. Concepto de innovación (qué es Marca Nexo, diferenciador)
6. Estrategia de canales y precios (tabla resumen)
7. Propuesta de comunicación y mensajes clave
8. Jerarquía de mensajes para punto de venta (3 niveles)
9. Plan de manejo de objeciones (modelo ACRA, resumen visual)
10. Plan de acción y cronograma
11. KPIs y métricas de seguimiento
12. Inversión y recursos requeridos
13. Criterios de éxito
14. Próximos pasos
15. Cierre y contacto

Tono: ejecutivo, visual, orientado a decisiones.
Usa gráficos y tablas donde sea posible en lugar de texto extenso.
Incluye notas del presentador en cada diapositiva.
```

7. Presiona **Enter** y espera a que Copilot genere la presentación (puede tardar 30-60 segundos).

8. Una vez generada, revisa rápidamente la cantidad de diapositivas y la estructura general.

**Resultado Esperado:**

PowerPoint mostrará una presentación de 12-15 diapositivas con:
- Diseño profesional aplicado automáticamente.
- Contenido extraído y sintetizado del Brief de Innovación.
- Tablas y elementos visuales en diapositivas de datos.
- Notas del presentador en el panel inferior de cada diapositiva.

**Verificación:**

- [ ] La presentación tiene entre 12 y 15 diapositivas.
- [ ] La diapositiva 1 es una portada con título del proyecto.
- [ ] La diapositiva 2 contiene una agenda o índice.
- [ ] Al menos 3 diapositivas contienen tablas o elementos gráficos.
- [ ] Las notas del presentador están pobladas (verificar en **Vista** → **Notas**).

---

#### Paso 5: Refinar diapositivas clave con prompts específicos

**Objetivo:** Mejorar diapositivas individuales utilizando las funciones de Copilot para agregar contenido, reorganizar información y optimizar el diseño visual.

**Instrucciones:**

1. **Diapositiva de Contexto Competitivo (diap. 3):** Navega a esta diapositiva, selecciónala y escribe en el panel de Copilot:

```text
Mejora esta diapositiva de contexto competitivo:
- Convierte el texto en una tabla comparativa de 3 columnas: 
  [Marca Nexo | Competidor A | Competidor B]
- Filas: Precio promedio, Canal principal, Beneficio clave, 
  Participación estimada
- Agrega un insight clave debajo de la tabla en formato de callout
- Mantén las notas del presentador con datos de soporte
```

2. Presiona **Enter** y revisa el resultado. Si la tabla no se visualiza correctamente, selecciona el contenido y pide: `Reorganiza esta información en un SmartArt de tipo tabla.`

3. **Diapositiva de Jerarquía de Mensajes (diap. 8):** Navega a esta diapositiva y escribe:

```text
Rediseña esta diapositiva usando un diagrama de pirámide invertida 
con 3 niveles:
- Base (más ancha): Nivel 1 — Mensaje primario de impacto (6 palabras)
- Centro: Nivel 2 — Beneficio principal (20 palabras)  
- Punta: Nivel 3 — Argumento de soporte y CTA (40 palabras)

A la derecha de la pirámide, muestra el soporte físico correspondiente 
a cada nivel: exhibidor, cenefa y folleto.
Usa los mensajes específicos de Marca Nexo del documento fuente.
```

4. **Diapositiva de KPIs (diap. 11):** Navega a esta diapositiva y escribe:

```text
Transforma los KPIs de esta diapositiva en un dashboard visual:
- Usa íconos o formas para representar cada KPI
- Incluye: meta numérica, plazo y responsable
- Máximo 6 KPIs en la diapositiva
- Formato: tarjetas visuales (card layout) en cuadrícula 2x3
Actualiza las notas del presentador con el detalle de cómo se medirá cada KPI.
```

5. **Agregar una diapositiva de transición:** Posiciona el cursor entre la diapositiva de estrategia de canales y la de comunicación. En Copilot escribe:

```text
Agrega una diapositiva de transición entre la estrategia comercial 
y la propuesta de comunicación con el texto:
"De la estrategia al mensaje: cómo llevar Marca Nexo al punto de venta"
Usa un diseño visual impactante con imagen de fondo sugerida.
```

6. Guarda la presentación: **Ctrl + S**.

**Resultado Esperado:**

Las diapositivas clave ahora tienen:
- Tabla comparativa competitiva en la diapositiva 3.
- Diagrama de pirámide invertida para jerarquía de mensajes en la diapositiva 8.
- Dashboard visual de KPIs en la diapositiva 11.
- Diapositiva de transición con diseño visual.

**Verificación:**

- [ ] La diapositiva de contexto competitivo contiene una tabla comparativa legible.
- [ ] La diapositiva de jerarquía de mensajes muestra los 3 niveles visualmente diferenciados.
- [ ] La diapositiva de KPIs presenta máximo 6 indicadores en formato visual.
- [ ] Existe una diapositiva de transición entre las secciones de estrategia y comunicación.

---

#### Paso 6: Generar y optimizar notas del presentador

**Objetivo:** Asegurar que todas las diapositivas tengan notas del presentador completas, con puntos de conversación y datos de soporte para una presentación fluida ante el comité directivo.

**Instrucciones:**

1. Ve a **Vista** → **Página de notas** para visualizar las notas de cada diapositiva.

2. Regresa a la vista **Normal**. Abre el panel de Copilot y escribe:

```text
Revisa las notas del presentador de TODAS las diapositivas de esta 
presentación y para cada una asegúrate de que incluyan:
1. Un punto de apertura (cómo introducir la diapositiva, máx. 1 oración)
2. Los 2-3 puntos clave a comunicar verbalmente
3. Un dato o evidencia de soporte que no esté en la diapositiva visible
4. Una frase de transición hacia la siguiente diapositiva

Tono: profesional pero natural, como si hablaras ante un comité 
directivo de una empresa de consumo masivo.
Extensión por diapositiva: 60-100 palabras en notas.
```

3. Presiona **Enter** y espera a que Copilot actualice las notas.

4. Navega por al menos 5 diapositivas verificando que las notas contengan los 4 elementos solicitados.

5. Si alguna diapositiva tiene notas insuficientes, posiciónate en ella y escribe:

```text
Mejora las notas del presentador de esta diapositiva específica. 
Incluye un dato cuantitativo relevante del Brief de Innovación 
y una pregunta retórica para generar engagement con la audiencia.
```

6. Guarda la presentación: **Ctrl + S**.

**Resultado Esperado:**

Todas las diapositivas tienen notas del presentador con los 4 elementos: apertura, puntos clave, dato de soporte y transición.

**Verificación:**

- [ ] Al menos 10 diapositivas tienen notas del presentador con 60-100 palabras.
- [ ] Las notas incluyen datos cuantitativos (porcentajes, cifras, plazos).
- [ ] Las transiciones entre diapositivas son lógicas y fluidas.
- [ ] El archivo está guardado como `M4_Presentacion_Ejecutiva_Lanzamiento.pptx` en la ruta correcta.

---

### PARTE 3 — Comunicaciones Diferenciadas en Outlook (12 minutos)

---

#### Paso 7: Redactar e-mail interno al equipo directivo

**Objetivo:** Utilizar Copilot en Outlook para redactar un correo electrónico profesional dirigido al equipo directivo, presentando el plan de lanzamiento de Marca Nexo con los puntos ejecutivos clave.

**Instrucciones:**

1. Abre **Microsoft Outlook**.

2. Haz clic en **Nuevo correo** (o **Ctrl + N**).

3. En el campo **Para:** escribe tu propia dirección de correo (este es un ejercicio de práctica).

4. En el campo **Asunto:** escribe: `Plan de Lanzamiento Marca Nexo — Bebidas Funcionales: Aprobación Requerida`

5. Haz clic en el icono de **Copilot** en la barra de herramientas del nuevo correo (o selecciona **Borrador con Copilot**).

6. Escribe el siguiente prompt:

```text
Redacta un correo electivo dirigido al Comité Directivo de la empresa 
presentando el plan de lanzamiento de Marca Nexo (línea de bebidas 
funcionales con electrolitos, sin azúcar añadida).

Estructura del correo:
1. Saludo ejecutivo
2. Contexto: por qué este lanzamiento es estratégico (2 oraciones)
3. Resumen de la oportunidad de mercado (3 bullet points)
4. Inversión estimada y ROI esperado (placeholder si no hay datos exactos)
5. Solicitud concreta: aprobación del plan y asignación de presupuesto
6. Próximos pasos: reunión de kickoff propuesta para [próximo martes]
7. Adjuntos referenciados: Brief de Innovación y Presentación Ejecutiva
8. Cierre profesional

Tono: ejecutivo, conciso, orientado a la acción.
Extensión: 200-300 palabras.
El correo debe transmitir urgencia sin ser alarmista.
```

7. Presiona **Generar** y revisa el borrador.

8. Si necesitas ajustar el tono, usa las opciones de Copilot: **Más formal**, **Más corto** o **Más directo** según corresponda.

9. **No envíes el correo todavía.** Guárdalo como borrador: **Ctrl + S** o cierra el correo y confirma **Guardar**.

**Resultado Esperado:**

Un correo profesional de 200-300 palabras con estructura clara, bullet points para la oportunidad de mercado, solicitud concreta de aprobación y referencia a los documentos adjuntos.

**Verificación:**

- [ ] El correo tiene saludo ejecutivo apropiado.
- [ ] Contiene al menos 3 bullet points con la oportunidad de mercado.
- [ ] Incluye solicitud concreta de aprobación.
- [ ] Referencia los adjuntos (Brief y Presentación).
- [ ] La extensión está entre 200-300 palabras.
- [ ] El correo está guardado como borrador.

---

#### Paso 8: Redactar e-mail externo a distribuidores clave

**Objetivo:** Utilizar Copilot en Outlook para redactar un correo diferenciado dirigido a distribuidores clave, con información relevante para su rol en el lanzamiento.

**Instrucciones:**

1. Crea un **Nuevo correo** en Outlook (**Ctrl + N**).

2. En **Para:** escribe tu propia dirección de correo.

3. En **Asunto:** escribe: `Marca Nexo — Nueva Oportunidad de Negocio: Bebidas Funcionales de Alta Rotación`

4. Activa **Copilot** en el correo y escribe:

```text
Redacta un correo dirigido a distribuidores clave (gerentes comerciales 
de distribuidoras regionales) presentando la nueva línea de bebidas 
funcionales Marca Nexo.

El correo debe ser COMPLETAMENTE DIFERENTE al correo interno directivo.
Enfoque: oportunidad de negocio para el distribuidor.

Estructura:
1. Saludo profesional pero cercano
2. Presentación breve de Marca Nexo (2 oraciones)
3. Por qué es una oportunidad para el distribuidor:
   - Margen atractivo (mencionar que es superior al promedio de categoría)
   - Soporte de marketing en punto de venta incluido
   - Materiales POP y capacitación para promotores sin costo
4. Condiciones de lanzamiento:
   - Pedido mínimo introductorio con descuento por volumen
   - Periodo de prueba de 60 días con devolución garantizada
5. Llamada a la acción: agendar reunión de presentación esta semana
6. Cierre con datos de contacto

Tono: profesional pero comercial, enfocado en beneficios para el 
distribuidor, no en características del producto.
Extensión: 180-250 palabras.
Incluye al final una posdata (P.D.) con un dato de mercado impactante 
sobre el crecimiento de la categoría de bebidas funcionales.
```

5. Presiona **Generar** y revisa el borrador.

6. Compara mentalmente este correo con el del Paso 7. Deben ser notablemente diferentes en tono, contenido y enfoque.

7. Guarda como borrador: **Ctrl + S**.

**Resultado Esperado:**

Un correo comercial de 180-250 palabras con enfoque en beneficios para el distribuidor (margen, soporte, condiciones), tono diferente al correo directivo, y una posdata con dato de mercado.

**Verificación:**

- [ ] El tono es comercial y orientado a beneficios del distribuidor (no del consumidor).
- [ ] Incluye condiciones comerciales concretas (descuento, periodo de prueba).
- [ ] Contiene llamada a la acción específica (agendar reunión).
- [ ] Incluye posdata con dato de mercado.
- [ ] Es claramente diferente en tono y contenido respecto al correo del Paso 7.
- [ ] El correo está guardado como borrador.

---

### PARTE 4 — Automatización en Microsoft Teams (9 minutos)

---

#### Paso 9: Simular y generar resumen de reunión de kickoff con Copilot en Teams

**Objetivo:** Utilizar Copilot en Microsoft Teams para generar el resumen estructurado de una reunión de kickoff del lanzamiento de Marca Nexo, incluyendo acuerdos, decisiones y asignación de tareas.

**Instrucciones:**

1. Abre **Microsoft Teams** (New Teams).

2. Navega al **Chat de Copilot** dentro de Teams:
   - Haz clic en el icono de **Copilot** en la barra lateral izquierda de Teams.
   - Si no aparece, búscalo en la barra de búsqueda superior escribiendo "Copilot".

3. En el chat de Copilot dentro de Teams, escribe el siguiente prompt para simular la generación de un resumen de reunión de kickoff:

```text
Actúa como asistente ejecutivo que documenta reuniones de negocio.

Genera el resumen completo de la reunión de kickoff del lanzamiento 
de Marca Nexo (bebidas funcionales) que acaba de concluir.

Participantes de la reunión:
- María López, Directora de Marketing (sponsor del proyecto)
- Carlos Ruiz, Gerente de Trade Marketing (líder de ejecución en PDV)
- Ana Torres, Gerente de Ventas Nacional (relación con distribuidores)
- Roberto Méndez, Director Financiero (aprobación de presupuesto)
- Laura Díaz, Coordinadora de Comunicaciones (gestión de mensajes)

Genera el resumen con esta estructura:
1. DATOS DE LA REUNIÓN: fecha (hoy), duración (45 min), modalidad (Teams)
2. OBJETIVO DE LA REUNIÓN: alinear al equipo en el plan de lanzamiento
3. DECISIONES TOMADAS (mínimo 5):
   - Aprobación del presupuesto de lanzamiento
   - Fecha de inicio de distribución
   - Canales prioritarios para fase 1
   - Proveedor seleccionado para materiales POP
   - Fecha de capacitación a equipo de promotores
4. ACUERDOS Y COMPROMISOS (tabla con columnas: 
   Acuerdo | Responsable | Fecha límite | Estatus)
   Incluye mínimo 8 acuerdos específicos y accionables.
5. RIESGOS IDENTIFICADOS (mínimo 3 con plan de mitigación)
6. PRÓXIMA REUNIÓN: fecha, agenda tentativa, participantes requeridos

Formato: profesional, listo para enviar por correo al equipo.
Usa viñetas y tablas para facilitar la lectura.
```

4. Presiona **Enter** y espera la generación.

5. Revisa el resumen generado. Verifica que:
   - Los acuerdos son específicos y tienen responsable asignado.
   - Las fechas límite son realistas.
   - Los riesgos tienen plan de mitigación concreto.

6. Si necesitas ajustar algún elemento, escribe un prompt de refinamiento:

```text
Modifica el resumen anterior:
- Agrega un acuerdo específico sobre la creación de la guía de manejo 
  de objeciones (modelo ACRA) para el equipo de promotores, asignado 
  a Carlos Ruiz con fecha límite de 2 semanas.
- En los riesgos, incluye el riesgo de baja rotación inicial y el plan 
  de mitigación basado en el periodo de prueba de 60 días con distribuidores.
```

7. **Copia el resumen final** (selecciona todo el texto → **Ctrl + C**).

8. Abre **Microsoft Word**, crea un nuevo documento y pega el contenido (**Ctrl + V**).

9. Guarda el archivo como `M4_Resumen_Kickoff_Lanzamiento.docx` en `Documentos/CopilotComunicacionEstrategia/M4_Brief_Presentacion/`.

> **💡 Nota sobre reuniones reales:** En un escenario real con una reunión de Teams grabada, Copilot genera automáticamente el resumen desde la transcripción. En este laboratorio simulamos el proceso porque no realizamos una reunión real. La estructura y los prompts son idénticos a los que usarías post-reunión con la función "Resumen de la reunión" de Copilot en Teams.

**Resultado Esperado:**

Un documento de resumen de reunión profesional con:
- 5+ decisiones tomadas.
- Tabla de 8+ acuerdos con responsable, fecha y estatus.
- 3+ riesgos con plan de mitigación.
- Fecha de próxima reunión con agenda tentativa.

**Verificación:**

- [ ] El resumen contiene los 6 elementos de estructura solicitados.
- [ ] La tabla de acuerdos tiene mínimo 8 filas con todas las columnas completas.
- [ ] Cada acuerdo tiene un responsable nombrado del equipo listado.
- [ ] Los riesgos incluyen planes de mitigación concretos.
- [ ] El documento está guardado en la ruta correcta de OneDrive.
- [ ] El resumen incluye el acuerdo sobre la guía ACRA para promotores.

---

## Validación y Pruebas Finales

Al completar todas las partes del laboratorio, realiza la siguiente validación integral de tu portafolio de entregables:

### Lista de Verificación de Archivos

| # | Archivo | Ruta en OneDrive | Estado |
|---|---------|------------------|--------|
| 1 | `M1_Informe_Ejecutivo_Posicionamiento.docx` | `…/M1_Informe_Ejecutivo/` | ☐ Presente y completo |
| 2 | `M2_Estrategia_Comercial_Precios.xlsx` | `…/M2_Estrategia_Comercial/` | ☐ Presente y completo |
| 3 | `M3_Kit_Comunicacion_Distribuidores.docx` | `…/M3_Kit_Comunicacion/` | ☐ Presente y completo |
| 4 | `M4_Brief_Innovacion.docx` | `…/M4_Brief_Presentacion/` | ☐ Creado en este lab |
| 5 | `M4_Presentacion_Ejecutiva_Lanzamiento.pptx` | `…/M4_Brief_Presentacion/` | ☐ Creado en este lab |
| 6 | Borrador de correo interno (Outlook) | Carpeta Borradores | ☐ Guardado |
| 7 | Borrador de correo a distribuidores (Outlook) | Carpeta Borradores | ☐ Guardado |
| 8 | `M4_Resumen_Kickoff_Lanzamiento.docx` | `…/M4_Brief_Presentacion/` | ☐ Creado en este lab |

### Validación de Calidad del Brief de Innovación

Abre `M4_Brief_Innovacion.docx` y confirma:

- [ ] **Portada** con título, subtítulo, autor y fecha.
- [ ] **Tabla de contenido** funcional (haz clic en una entrada para verificar que navega a la sección correcta).
- [ ] **8 secciones** con encabezados de Nivel 2 correctamente formateados.
- [ ] **Tabla de KPIs** en la sección 6 con al menos 5 indicadores medibles.
- [ ] **Cronograma** en la sección 7 en formato de tabla.
- [ ] **Jerarquía de mensajes** con 3 niveles y variantes de lanzamiento.
- [ ] **Argumentario ACRA** con 6 respuestas (3 objeciones × 2 audiencias).
- [ ] **Extensión total** entre 1,500 y 2,500 palabras (verificar en **Revisar** → **Contar palabras**).

### Validación de Calidad de la Presentación Ejecutiva

Abre `M4_Presentacion_Ejecutiva_Lanzamiento.pptx` y confirma:

- [ ] **12-15 diapositivas** en total.
- [ ] **Portada** con nombre del proyecto y fecha.
- [ ] **Diapositiva de agenda** que refleja la estructura completa.
- [ ] **Tabla comparativa competitiva** en la diapositiva de contexto.
- [ ] **Diagrama de jerarquía de mensajes** visualmente diferenciado por niveles.
- [ ] **Dashboard de KPIs** con formato visual (no solo texto).
- [ ] **Notas del presentador** en al menos 10 diapositivas con los 4 elementos (apertura, puntos clave, dato de soporte, transición).
- [ ] **Diapositiva de transición** entre secciones de estrategia y comunicación.

### Validación de Diferenciación de Correos

Compara ambos borradores en Outlook y confirma:

- [ ] El correo interno usa tono **ejecutivo-estratégico** y solicita aprobación.
- [ ] El correo externo usa tono **comercial-relacional** y ofrece oportunidad de negocio.
- [ ] Los mensajes clave son **diferentes** aunque se refieren al mismo producto.
- [ ] Cada correo tiene una **llamada a la acción** distinta y apropiada para su audiencia.

---

## Solución de Problemas

### Problema 1: Copilot no encuentra los archivos referenciados al usar "/" en el prompt

**Síntomas:** Al escribir `/` en el panel de Copilot (Word o PowerPoint) para referenciar archivos de módulos anteriores, la lista desplegable no muestra los archivos M1, M2 o M3, o muestra el mensaje "No se encontraron archivos".

**Causa:** Los archivos no están sincronizados correctamente en OneDrive, están en una ubicación diferente a la esperada, o la indexación de Microsoft 365 aún no los ha procesado (puede tardar hasta 15 minutos después de guardar un archivo nuevo en OneDrive).

**Solución:**

1. Abre **Explorador de archivos** → navega a la carpeta de OneDrive y verifica que los archivos M1, M2 y M3 muestren el ícono de **nube con check verde** (sincronizados) y no una nube con flecha o un ícono de error.
2. Si los archivos muestran estado pendiente, haz clic derecho en el ícono de OneDrive en la bandeja del sistema → **Configuración** → **Cuenta** → **Elegir carpetas** y confirma que la carpeta `CopilotComunicacionEstrategia` está seleccionada para sincronización.
3. Abre cada archivo directamente desde OneDrive en el navegador (ve a `onedrive.com`, navega a la carpeta y abre el archivo). Esto fuerza la indexación.
4. Espera 2-3 minutos y vuelve a intentar el comando `/` en Copilot.
5. Si el problema persiste, copia la **URL completa de OneDrive** del archivo (clic derecho → **Copiar vínculo** en OneDrive web) y pégala directamente en el prompt de Copilot en lugar de usar `/`.
6. Como último recurso, abre el archivo fuente (por ejemplo, M1) en una pestaña de Word y en el prompt de Copilot referencia "el documento abierto en la otra pestaña" o copia y pega las secciones clave directamente en el prompt.

---

### Problema 2: La presentación generada por Copilot en PowerPoint tiene menos de 10 diapositivas o contenido incompleto

**Síntomas:** Al ejecutar el prompt de creación de presentación desde archivo en PowerPoint, Copilot genera solo 5-7 diapositivas en lugar de las 12-15 solicitadas, omite secciones completas del brief, o las diapositivas contienen solo títulos sin contenido.

**Causa:** Copilot en PowerPoint tiene un límite de procesamiento por prompt y puede truncar la generación cuando el documento fuente es extenso o cuando el prompt solicita demasiadas diapositivas específicas en una sola instrucción. También puede ocurrir si el Brief de Innovación no está completamente guardado/sincronizado al momento de referenciarlo.

**Solución:**

1. **Verifica la sincronización:** Confirma que `M4_Brief_Innovacion.docx` está completamente guardado y sincronizado en OneDrive (ícono de check verde) antes de referenciarlo desde PowerPoint.
2. **Divide la generación en dos fases.** Primero, genera las diapositivas 1-8 con un prompt enfocado en la primera mitad del brief:

```text
Crea una presentación a partir de /M4_Brief_Innovacion.docx.
Genera las primeras 8 diapositivas cubriendo: portada, agenda, 
contexto competitivo, oportunidad de mercado, concepto de innovación, 
estrategia de canales, propuesta de comunicación y jerarquía de mensajes.
```

3. Luego, usa la función **"Agregar una diapositiva"** de Copilot para generar las diapositivas restantes una por una o en grupos pequeños:

```text
Agrega una diapositiva sobre el plan de acción y cronograma de 
lanzamiento, basándote en la sección 7 del archivo 
/M4_Brief_Innovacion.docx. Incluye una tabla tipo timeline.
```

4. Repite el proceso para cada sección faltante (KPIs, recursos, criterios de éxito, próximos pasos, cierre).
5. Si las diapositivas tienen solo títulos sin contenido, selecciona cada una y usa Copilot con: `Completa el contenido de esta diapositiva con información relevante del Brief de Innovación. Incluye bullet points concisos y una tabla o gráfico si aplica.`

---

## Limpieza del Entorno

Al finalizar el laboratorio:

1. **Verifica la sincronización final** de todos los archivos en OneDrive:
   - Abre el Explorador de archivos → navega a `OneDrive/Documentos/CopilotComunicacionEstrategia/M4_Brief_Presentacion/`.
   - Confirma que los 3 archivos del módulo 4 están presentes y sincronizados:
     - `M4_Brief_Innovacion.docx`
     - `M4_Presentacion_Ejecutiva_Lanzamiento.pptx`
     - `M4_Resumen_Kickoff_Lanzamiento.docx`

2. **Cierra las aplicaciones** que no necesites para liberar memoria:
   - Cierra las pestañas adicionales de Word y PowerPoint que no sean los archivos finales.
   - Mantén Outlook abierto solo si necesitas revisar los borradores.

3. **Borradores de Outlook:** Los correos de práctica están en tu carpeta de Borradores. Puedes:
   - **Conservarlos** como referencia para uso futuro.
   - **Eliminarlos** si no los necesitas (Borradores → seleccionar → Eliminar).

4. **No elimines** ningún archivo de los módulos M1, M2 o M3, ya que forman parte del portafolio completo del curso.

5. **Historial de Copilot en Teams:** El chat con Copilot se conserva automáticamente. No requiere limpieza.

---

## Resumen

### Lo que construiste en este laboratorio

En 72 minutos completaste el ciclo end-to-end de producción ejecutiva con Microsoft 365 Copilot:

| Parte | Herramienta | Entregable | Tiempo |
|-------|-------------|------------|--------|
| 1 | Word + Copilot | Brief de Innovación con jerarquía de mensajes y modelo ACRA | 25 min |
| 2 | PowerPoint + Copilot | Presentación Ejecutiva de 12-15 diapositivas con notas del presentador | 30 min |
| 3 | Outlook + Copilot | 2 correos diferenciados (interno ejecutivo + externo comercial) | 12 min |
| 4 | Teams + Copilot | Resumen de reunión de kickoff con acuerdos y responsables | 9 min |

### Conceptos clave aplicados

- **Referenciación cross-documento:** Utilizaste archivos de módulos anteriores como contexto para Copilot, demostrando el flujo integrado Word → PowerPoint → Outlook → Teams.
- **Jerarquía de mensajes:** Integraste los 3 niveles (primario, secundario, soporte) del punto de venta directamente en el brief y la presentación.
- **Modelo ACRA:** Generaste argumentarios de manejo de objeciones diferenciados por audiencia (gerente de categoría vs. consumidor final).
- **Diferenciación por audiencia:** Los dos correos de Outlook demuestran cómo Copilot adapta tono, contenido y llamada a la acción según el destinatario.
- **Ingeniería de prompts avanzada:** Cada prompt incluyó rol, contexto, estructura, tono, extensión y formato de salida para obtener resultados consistentes y profesionales.

### Portafolio final del curso

Al completar este laboratorio, tu portafolio de 5 entregables profesionales es:

1. **M1** — Informe Ejecutivo de Posicionamiento (Word)
2. **M2** — Estrategia Comercial y Modelo de Precios (Excel)
3. **M3** — Kit de Comunicación para Distribuidores (Word)
4. **M4** — Brief de Innovación (Word) + Presentación Ejecutiva de Lanzamiento (PowerPoint)
5. **Bonus M4** — Correos diferenciados (Outlook) + Resumen de kickoff (Teams/Word)

### Recursos Adicionales

- [Documentación oficial: Copilot en Word](https://support.microsoft.com/es-es/copilot-word)
- [Documentación oficial: Copilot en PowerPoint](https://support.microsoft.com/es-es/copilot-powerpoint)
- [Documentación oficial: Copilot en Outlook](https://support.microsoft.com/es-es/copilot-outlook)
- [Documentación oficial: Copilot en Teams](https://support.microsoft.com/es-es/copilot-teams)
- [Guía de ingeniería de prompts para Microsoft 365 Copilot](https://adoption.microsoft.com/es-es/copilot/)
- [Modelo ACRA para manejo de objeciones — HubSpot](https://blog.hubspot.es/sales/manejo-de-objeciones)
