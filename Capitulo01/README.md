# Práctica: Creación de un informe ejecutivo de posicionamiento y análisis de portafolio competitivo utilizando Copilot

## Metadatos del Laboratorio

| Campo | Detalle |
|---|---|
| **Duración** | 72 minutos |
| **Complejidad** | Media |
| **Nivel de Bloom** | Crear |
| **Módulo** | M1 — Informe Ejecutivo |
| **Archivo de salida** | `M1_Informe_Ejecutivo_Posicionamiento.docx` |

---

## Descripción General

En este laboratorio construirás desde cero un informe ejecutivo de posicionamiento competitivo utilizando Microsoft Word con Copilot. Aplicarás el marco de ingeniería de prompts **RCTF (Rol, Contexto, Tarea, Formato)** para generar análisis de tendencias de mercado, una matriz de benchmarking de competidores, un mapa de posicionamiento conceptual y una propuesta de valor diferenciada. Este es el primer laboratorio del curso y establece tanto la estructura de archivos en OneDrive como la metodología de prompts que utilizarás en los módulos 2, 3 y 4. El documento generado aquí será insumo directo para el Módulo 2.

---

## Objetivos de Aprendizaje

Al completar este laboratorio serás capaz de:

- [ ] Crear y organizar la estructura completa de carpetas en OneDrive que servirá como repositorio de trabajo para los cuatro módulos del curso.
- [ ] Aplicar el marco RCTF (Rol, Contexto, Tarea, Formato) con restricciones y variables para generar análisis de mercado estructurados mediante Copilot en Word.
- [ ] Construir un informe ejecutivo completo que incluya resumen ejecutivo, análisis de tendencias, matriz de benchmarking de al menos 3 competidores, análisis de brechas y propuesta de valor diferenciada.
- [ ] Utilizar técnicas de encadenamiento de prompts (prompt chaining) e iteración para refinar progresivamente la profundidad y calidad de los outputs de Copilot.
- [ ] Validar y editar críticamente los contenidos generados por IA, asegurando coherencia estratégica y calidad profesional del documento final.

---

## Prerrequisitos

### Conocimientos Previos

| Requisito | Nivel |
|---|---|
| Navegación básica en Microsoft Word (abrir, guardar, cinta de opciones) | Requerido |
| Comprensión conceptual de análisis competitivo y propuesta de valor | Requerido |
| Familiaridad con OneDrive (navegación de carpetas, sincronización) | Requerido |
| Experiencia previa con Copilot | No requerido |

### Acceso y Licencias

| Elemento | Estado requerido |
|---|---|
| Cuenta corporativa Microsoft 365 | Activa y con sesión iniciada |
| Licencia **Microsoft Copilot for Microsoft 365** | Asignada y verificada en admin.microsoft.com |
| OneDrive for Business | Sincronizado y con al menos 1 GB de espacio disponible |
| Conexión a internet | Estable, mínimo 10 Mbps descarga / 5 Mbps subida |

> ⚠️ **Importante:** Sin la licencia de Copilot for Microsoft 365 asignada individualmente, no podrás ejecutar ningún paso de este laboratorio. Verifica con tu instructor antes de comenzar.

---

## Entorno del Laboratorio

### Hardware Mínimo

| Componente | Especificación |
|---|---|
| Procesador | Intel Core i5 8ª gen. / AMD Ryzen 5 3000 o superior |
| RAM | 8 GB mínimo (16 GB recomendado) |
| Almacenamiento | 10 GB disponibles (SSD recomendado) |
| Pantalla | 1366×768 mínimo (1920×1080 recomendado) |
| Periféricos | Ratón externo recomendado |

### Software Requerido

| Aplicación | Versión mínima |
|---|---|
| Microsoft 365 Apps for Enterprise | Versión 2405 (Build 17628.20144) — Canal Mensual |
| Microsoft Copilot for Microsoft 365 | Release de servicio mayo 2024 o posterior |
| OneDrive for Business (cliente de sincronización) | Versión 24.071.0407.0003 o superior |
| Microsoft Edge | 126.0.2592.68 o superior |

### Verificación Rápida del Entorno

Antes de comenzar, ejecuta estas comprobaciones:

1. Abre **Microsoft Word** → **Archivo** → **Cuenta** → Verifica que la versión sea 2405 o superior.
2. En un documento nuevo de Word, busca el ícono de **Copilot** en la cinta de opciones (pestaña **Inicio**). Si no aparece, tu licencia no está activa.
3. Abre el **Explorador de archivos** → Verifica que OneDrive aparezca en el panel lateral izquierdo con el ícono de nube azul y estado "Sincronizado".

---

## Instrucciones Paso a Paso

### Paso 1 — Crear la estructura de carpetas del curso en OneDrive

**Objetivo:** Establecer el repositorio de trabajo organizado que se usará durante los cuatro módulos del curso.

**Tiempo estimado:** 5 minutos

**Instrucciones:**

1. Abre el **Explorador de archivos** de Windows y navega a tu carpeta de **OneDrive** → **Documentos**.

2. Crea la carpeta raíz del curso:
   - Clic derecho → **Nuevo** → **Carpeta** → Nombra: `CopilotComunicacionEstrategia`

3. Dentro de `CopilotComunicacionEstrategia`, crea las siguientes cuatro subcarpetas:

   ```
   CopilotComunicacionEstrategia/
   ├── M1_Informe_Ejecutivo/
   ├── M2_Estrategia_Comercial/
   ├── M3_Kit_Comunicacion/
   └── M4_Brief_Presentacion/
   ```

4. Verifica que OneDrive sincronice las carpetas (aparecerá una marca de verificación verde ✅ o un ícono de nube azul junto a cada carpeta).

5. Navega a la carpeta `M1_Informe_Ejecutivo/` y déjala abierta; aquí guardarás el archivo principal de este laboratorio.

**Resultado esperado:** Cuatro subcarpetas creadas dentro de `Documentos/CopilotComunicacionEstrategia/`, todas sincronizadas con OneDrive.

**Verificación:**
- Abre un navegador → Ingresa a [onedrive.com](https://onedrive.com) → Navega a **Documentos** → Confirma que la estructura de carpetas aparece idéntica en la nube.
- Las cuatro subcarpetas deben ser visibles: `M1_Informe_Ejecutivo`, `M2_Estrategia_Comercial`, `M3_Kit_Comunicacion`, `M4_Brief_Presentacion`.

---

### Paso 2 — Crear el documento base y configurar el entorno de trabajo en Word

**Objetivo:** Crear el archivo `M1_Informe_Ejecutivo_Posicionamiento.docx` y familiarizarse con la interfaz de Copilot en Word.

**Tiempo estimado:** 5 minutos

**Instrucciones:**

1. Abre **Microsoft Word** desde el menú de inicio o la barra de tareas.

2. Selecciona **Documento en blanco**.

3. Guarda inmediatamente el archivo:
   - **Archivo** → **Guardar como** → **OneDrive** → Navega a `Documentos/CopilotComunicacionEstrategia/M1_Informe_Ejecutivo/`
   - Nombre del archivo: `M1_Informe_Ejecutivo_Posicionamiento`
   - Formato: **Documento de Word (.docx)**
   - Haz clic en **Guardar**.

4. Verifica que en la barra de título de Word aparezca el nombre del archivo seguido de "Guardado" o el ícono de OneDrive.

5. Localiza el botón de **Copilot** en la cinta de opciones:
   - En la pestaña **Inicio**, busca el ícono de Copilot (generalmente a la derecha de la cinta).
   - Haz clic en él para abrir el **panel lateral de Copilot**.

6. Verifica que el panel lateral de Copilot se abra correctamente en el lado derecho de la pantalla. Deberías ver un campo de texto con el placeholder "Pregúntame cualquier cosa sobre este documento" o similar.

7. Adicionalmente, coloca el cursor al inicio del documento vacío. Deberías ver la opción flotante **"Borrador con Copilot"** (un ícono de Copilot con texto que invita a redactar). Esta es la función que usarás para generar contenido directamente en el cuerpo del documento.

**Resultado esperado:** Documento `M1_Informe_Ejecutivo_Posicionamiento.docx` guardado en la ubicación correcta de OneDrive, con el panel lateral de Copilot abierto y la función "Borrador con Copilot" disponible en el cuerpo del documento.

**Verificación:**
- La barra de título muestra: `M1_Informe_Ejecutivo_Posicionamiento — Guardado en OneDrive`.
- El panel lateral de Copilot está visible y responde al escribir un texto de prueba (puedes escribir "Hola" y verificar que responde; luego borra esa interacción).

---

### Paso 3 — Generar el resumen ejecutivo y análisis de tendencias del mercado

**Objetivo:** Utilizar la función "Borrador con Copilot" para generar las dos primeras secciones del informe aplicando el marco RCTF con restricciones específicas.

**Tiempo estimado:** 12 minutos

**Instrucciones:**

1. Asegúrate de que el cursor esté al inicio del documento vacío. Haz clic en la opción **"Borrador con Copilot"** que aparece en el cuerpo del documento (o usa el atajo: simplemente comienza a escribir en el campo de Copilot que aparece).

2. En el cuadro de texto de "Borrador con Copilot", escribe el siguiente prompt **exactamente** como aparece (puedes sustituir los valores entre corchetes si deseas usar tu propia industria, pero para este laboratorio se recomienda usar el caso guía):

   ```text
   Actúa como un analista de inteligencia de mercado senior con 15 años de experiencia en el sector de bebidas funcionales en América Latina.

   Contexto: Marca Nexo es una empresa mexicana que produce una línea de bebidas funcionales premium (energía, hidratación y bienestar) dirigida a adultos de 25-45 años, nivel socioeconómico ABC+, distribuida en canal moderno (supermercados y tiendas de conveniencia). Compite en un mercado en crecimiento estimado del 12% anual.

   Tarea: Genera las dos primeras secciones de un informe ejecutivo de posicionamiento:

   SECCIÓN 1 — Resumen Ejecutivo: Un resumen de máximo 1 página que describa la situación actual del mercado de bebidas funcionales en México, la posición de Marca Nexo y los principales desafíos y oportunidades identificados.

   SECCIÓN 2 — Análisis de Tendencias del Mercado: Identifica y describe las 5 tendencias más relevantes que están transformando la categoría de bebidas funcionales en México. Para cada tendencia incluye: nombre, descripción de 2-3 oraciones, evidencia o indicadores que la sustentan, y nivel de impacto (Alto / Medio / Bajo).

   Formato:
   - El resumen ejecutivo debe estar en prosa profesional con párrafos cortos.
   - Las tendencias deben presentarse en una tabla con columnas: Tendencia | Descripción | Evidencia/Indicadores | Nivel de Impacto.
   - Usa encabezados de nivel 2 (##) para cada sección.
   - Tono: ejecutivo, directo, sin jerga innecesaria.

   Restricciones: No incluyas datos numéricos inventados con fuentes específicas. Usa rangos estimados o indicadores cualitativos. Limita el análisis al mercado mexicano.
   ```

3. Haz clic en el botón **Generar** (o presiona **Enter** si el campo lo permite).

4. Espera a que Copilot genere el contenido. Esto puede tomar entre 10 y 30 segundos.

5. **Revisa el contenido generado** antes de aceptarlo:
   - ¿Incluye un encabezado de Resumen Ejecutivo?
   - ¿El resumen tiene un tono ejecutivo y no excede una página?
   - ¿Aparece una tabla de tendencias con las 4 columnas solicitadas?
   - ¿Se identifican 5 tendencias?

6. Si el resultado es satisfactorio, haz clic en **Conservar** (o **Keep**).

7. Si el resultado necesita ajustes, tienes dos opciones:
   - Haz clic en **Regenerar** para obtener una nueva versión completa.
   - Haz clic en **Conservar** y luego ajusta manualmente el texto, o utiliza la función "Reescribir con Copilot" en secciones específicas (se cubrirá en pasos posteriores).

8. Una vez conservado el contenido, presiona **Ctrl + S** para guardar.

**Resultado esperado:** El documento ahora contiene dos secciones claramente diferenciadas:
- **Resumen Ejecutivo** (~250-400 palabras en prosa profesional)
- **Análisis de Tendencias del Mercado** (tabla con 5 tendencias, 4 columnas cada una)

**Verificación:**
- El resumen ejecutivo menciona a Marca Nexo, el mercado de bebidas funcionales y al menos 2 desafíos u oportunidades.
- La tabla de tendencias tiene exactamente 4 columnas y al menos 5 filas de contenido.
- No hay datos con fuentes bibliográficas inventadas (conforme a la restricción del prompt).
- Los encabezados usan formato de Título 2 (Heading 2) de Word.

---

### Paso 4 — Generar la matriz de benchmarking competitivo mediante encadenamiento de prompts

**Objetivo:** Aplicar la técnica de encadenamiento de prompts (prompt chaining) para crear un análisis comparativo detallado de al menos 3 competidores directos de Marca Nexo.

**Tiempo estimado:** 15 minutos

**Instrucciones:**

1. Coloca el cursor al final del contenido generado en el Paso 3 (después de la tabla de tendencias). Presiona **Enter** dos veces para crear espacio.

2. Haz clic en la opción **"Borrador con Copilot"** que aparece en la nueva línea vacía.

3. Escribe el **primer prompt de la cadena** — identificación de competidores:

   ```text
   Actúa como consultor de inteligencia competitiva especializado en bebidas funcionales en México.

   Contexto: Estás construyendo la sección de benchmarking competitivo para el informe ejecutivo de Marca Nexo (bebidas funcionales premium, segmento ABC+, canal moderno en México). Las secciones anteriores de este documento ya incluyen el resumen ejecutivo y las tendencias del mercado.

   Tarea: Identifica los 4 competidores directos más relevantes para Marca Nexo en el mercado mexicano de bebidas funcionales. Para cada competidor proporciona: nombre de la marca, empresa matriz, segmento de precio (Premium / Medio / Económico), principales productos y una descripción de su posicionamiento en 2 oraciones.

   Formato: Tabla con columnas: Competidor | Empresa Matriz | Segmento de Precio | Productos Principales | Posicionamiento.
   Añade un encabezado de nivel 2: "## Benchmarking Competitivo".
   Incluye un párrafo introductorio de 2-3 oraciones antes de la tabla.

   Restricciones: Selecciona marcas reales que operen en México. Si no tienes certeza de un dato específico, indícalo como "por confirmar".
   ```

4. Haz clic en **Generar**. Revisa que la tabla contenga 4 competidores con las 5 columnas solicitadas. Haz clic en **Conservar**.

5. Ahora, coloca el cursor después de la tabla de competidores recién generada. Presiona **Enter** dos veces.

6. Haz clic en **"Borrador con Copilot"** nuevamente y escribe el **segundo prompt de la cadena** — análisis comparativo profundo:

   ```text
   Actúa como analista de posicionamiento de marcas con experiencia en consumo masivo.

   Contexto: Revisa la tabla de competidores que aparece en la sección anterior de este documento. Marca Nexo es nuestra marca y los competidores identificados son los que aparecen en dicha tabla.

   Tarea: Crea una matriz comparativa detallada que evalúe a Marca Nexo y a los 4 competidores identificados en los siguientes criterios:
   1. Propuesta de valor principal
   2. Público objetivo primario
   3. Canales de distribución principales
   4. Rango de precio estimado (por unidad de 500ml)
   5. Mensaje de comunicación predominante
   6. Presencia digital (Alta / Media / Baja)

   Formato:
   - Tabla comparativa con cada marca como columna y cada criterio como fila.
   - Después de la tabla, incluye un subtítulo "### Hallazgos Clave del Benchmarking" con 4 hallazgos numerados, cada uno de 2-3 oraciones.

   Restricciones: Para Marca Nexo, usa los siguientes datos: propuesta de valor = "rendimiento natural sin ingredientes artificiales", público = adultos 25-45 ABC+, canales = supermercados y tiendas de conveniencia, precio = $35-45 MXN por 500ml, mensaje = "Potencia tu día de forma natural".
   ```

7. Haz clic en **Generar**. Revisa el resultado:
   - ¿La tabla tiene 5 columnas (Marca Nexo + 4 competidores) y 6 filas de criterios?
   - ¿Los hallazgos clave son específicos y accionables?

8. Si algún hallazgo es demasiado genérico, selecciona ese texto específico, haz clic derecho y selecciona **Reescribir con Copilot**. En el cuadro que aparece, escribe:

   ```text
   Reescribe este hallazgo para que sea más específico y accionable. Incluye una implicación estratégica concreta para Marca Nexo.
   ```

9. Acepta la reescritura si mejora el contenido. Guarda el documento con **Ctrl + S**.

**Resultado esperado:** El documento ahora incluye una nueva sección "Benchmarking Competitivo" con:
- Párrafo introductorio
- Tabla de identificación de 4 competidores (5 columnas)
- Matriz comparativa detallada (5 columnas × 6 criterios)
- 4 hallazgos clave numerados

**Verificación:**
- La sección de benchmarking contiene exactamente 2 tablas (identificación + comparativa).
- Los datos de Marca Nexo en la matriz coinciden con las restricciones proporcionadas en el prompt.
- Los hallazgos mencionan al menos una brecha competitiva y una ventaja de Marca Nexo.
- El encadenamiento se evidencia: el segundo prompt referencia explícitamente la tabla del primero.

---

### Paso 5 — Crear el mapa de posicionamiento conceptual y el análisis de brechas

**Objetivo:** Generar una representación textual del posicionamiento competitivo y un análisis de brechas estratégicas utilizando prompts iterativos.

**Tiempo estimado:** 12 minutos

**Instrucciones:**

1. Coloca el cursor al final de la sección de benchmarking. Presiona **Enter** dos veces.

2. Haz clic en **"Borrador con Copilot"** y escribe el siguiente prompt para el mapa de posicionamiento:

   ```text
   Actúa como estratega de marca con experiencia en mapas perceptuales de posicionamiento.

   Contexto: Revisa las secciones anteriores de este documento, incluyendo la matriz de benchmarking de Marca Nexo y sus 4 competidores en bebidas funcionales en México.

   Tarea: Crea un mapa de posicionamiento conceptual que ubique a Marca Nexo y sus competidores en dos ejes:
   - Eje X: Precio (Económico → Premium)
   - Eje Y: Percepción de naturalidad/salud (Convencional → Natural/Saludable)

   Dado que no puedes generar un gráfico visual, describe el mapa de posicionamiento de la siguiente manera:
   1. Una tabla con columnas: Marca | Posición en Eje X (1-10) | Posición en Eje Y (1-10) | Cuadrante resultante.
   2. Una descripción narrativa de 1 párrafo por cuadrante, indicando qué marcas se ubican ahí y qué implica estratégicamente.

   Formato:
   - Encabezado nivel 2: "## Mapa de Posicionamiento Competitivo"
   - Tabla de coordenadas primero, luego descripciones por cuadrante.
   - Define los 4 cuadrantes como: "Premium-Natural" (superior derecho), "Premium-Convencional" (inferior derecho), "Económico-Natural" (superior izquierdo), "Económico-Convencional" (inferior izquierdo).

   Restricciones: Marca Nexo debe ubicarse en el cuadrante Premium-Natural. Asigna posiciones coherentes con la información de precio y propuesta de valor del benchmarking anterior.
   ```

3. Haz clic en **Generar**. Revisa que la tabla tenga valores numéricos coherentes y que las descripciones de cuadrantes sean estratégicamente relevantes. Haz clic en **Conservar**.

4. Ahora, coloca el cursor después del mapa de posicionamiento. Presiona **Enter** dos veces.

5. Haz clic en **"Borrador con Copilot"** y escribe el prompt para el análisis de brechas:

   ```text
   Actúa como director de estrategia comercial de una empresa de consumo masivo.

   Contexto: Revisa todo el contenido generado en las secciones anteriores de este documento: el resumen ejecutivo, las tendencias de mercado, el benchmarking competitivo y el mapa de posicionamiento de Marca Nexo.

   Tarea: Realiza un análisis de brechas estratégicas y oportunidades para Marca Nexo. Identifica:
   1. Tres brechas competitivas (áreas donde Marca Nexo está en desventaja frente a competidores).
   2. Tres oportunidades estratégicas (espacios de mercado no cubiertos o tendencias no aprovechadas).
   3. Para cada brecha y oportunidad, incluye: descripción, competidor o tendencia relacionada, nivel de urgencia (Alta / Media / Baja) y una acción recomendada de 1-2 oraciones.

   Formato:
   - Encabezado nivel 2: "## Análisis de Brechas y Oportunidades"
   - Dos tablas separadas: una para "Brechas Competitivas" y otra para "Oportunidades Estratégicas".
   - Columnas de cada tabla: # | Descripción | Referencia (competidor/tendencia) | Urgencia | Acción Recomendada.
   - Después de las tablas, un párrafo de síntesis de máximo 4 oraciones.

   Restricciones: Las brechas y oportunidades deben ser coherentes con los datos de las secciones anteriores. No repitas información ya cubierta; genera insights nuevos y accionables.
   ```

6. Haz clic en **Generar**. Revisa la coherencia:
   - ¿Las brechas referencian competidores mencionados en el benchmarking?
   - ¿Las oportunidades se conectan con las tendencias identificadas en el Paso 3?

7. Si alguna acción recomendada es vaga, selecciónala y usa **Reescribir con Copilot** con esta instrucción:

   ```text
   Hazla más concreta: incluye un canal específico, un plazo estimado o un KPI medible.
   ```

8. Conserva los cambios y guarda con **Ctrl + S**.

**Resultado esperado:** Dos nuevas secciones en el documento:
- **Mapa de Posicionamiento Competitivo** con tabla de coordenadas y descripciones por cuadrante
- **Análisis de Brechas y Oportunidades** con 2 tablas (3 brechas + 3 oportunidades) y párrafo de síntesis

**Verificación:**
- Marca Nexo aparece en el cuadrante Premium-Natural con valores de Eje X ≥ 7 y Eje Y ≥ 7.
- Las brechas mencionan al menos un competidor por nombre del benchmarking anterior.
- Las oportunidades referencian al menos una tendencia de la tabla del Paso 3.
- Las acciones recomendadas son específicas (mencionan canal, segmento o tipo de acción).

---

### Paso 6 — Generar la propuesta de valor diferenciada

**Objetivo:** Crear la sección final del informe con una propuesta de valor fundamentada en todo el análisis previo, utilizando el panel lateral de Copilot para un enfoque de consulta diferente.

**Tiempo estimado:** 10 minutos

**Instrucciones:**

1. Para esta sección, usarás el **panel lateral de Copilot** (no "Borrador con Copilot") para demostrar un flujo de trabajo diferente. Asegúrate de que el panel lateral esté abierto (haz clic en el ícono de Copilot en la cinta de opciones si no lo está).

2. En el campo de texto del panel lateral, escribe el siguiente prompt:

   ```text
   Basándote en todo el contenido de este documento, genera una sección titulada "Propuesta de Valor Diferenciada para Marca Nexo" que incluya:

   1. Un statement de posicionamiento en formato: "Para [público objetivo], Marca Nexo es la [categoría] que [beneficio principal] porque [razón para creer]."

   2. Tres pilares de diferenciación, cada uno con: nombre del pilar, descripción de 2-3 oraciones y cómo se conecta con las brechas u oportunidades identificadas en el análisis anterior.

   3. Un párrafo de cierre titulado "Ventaja Competitiva Sostenible" que explique por qué esta propuesta de valor es difícil de replicar por los competidores.

   Formato: Usa encabezados nivel 2 y nivel 3. El statement de posicionamiento debe estar en negrita y centrado. Tono: estratégico y persuasivo, adecuado para una presentación a comité directivo.
   ```

3. Copilot generará la respuesta en el panel lateral. **Revisa el contenido** en el panel antes de insertarlo.

4. Para insertar el contenido en el documento, haz clic en el botón **Copiar** que aparece debajo de la respuesta en el panel lateral.

5. Coloca el cursor al final del documento (después del análisis de brechas) y pega el contenido con **Ctrl + V**.

6. **Ajusta el formato** manualmente:
   - Selecciona el título "Propuesta de Valor Diferenciada para Marca Nexo" y aplícale estilo **Título 2** desde la cinta de opciones.
   - Selecciona los nombres de los pilares y aplícales estilo **Título 3**.
   - Selecciona el statement de posicionamiento, aplícale **negrita** (Ctrl + B) y **centrado** (Ctrl + E).

7. Si deseas refinar el statement de posicionamiento, selecciónalo en el documento, haz clic derecho y elige **Reescribir con Copilot**. Escribe:

   ```text
   Reescribe este statement para que sea más memorable y emocionalmente resonante, manteniendo la estructura "Para [público], Marca Nexo es... que... porque...". Hazlo en máximo 2 oraciones.
   ```

8. Acepta la versión que consideres más fuerte. Guarda con **Ctrl + S**.

**Resultado esperado:** Sección final del informe con:
- Statement de posicionamiento en formato estándar, en negrita y centrado
- 3 pilares de diferenciación con conexión explícita al análisis previo
- Párrafo de ventaja competitiva sostenible

**Verificación:**
- El statement de posicionamiento sigue la estructura "Para... es la... que... porque..."
- Cada pilar de diferenciación referencia al menos una brecha u oportunidad del análisis anterior.
- El párrafo de ventaja competitiva menciona al menos un factor difícil de replicar.
- Los estilos de encabezado son consistentes con el resto del documento (Título 2 y Título 3).

---

### Paso 7 — Revisar, refinar y validar el documento completo

**Objetivo:** Utilizar Copilot para resumir el documento, verificar coherencia interna y aplicar ajustes finales de calidad profesional.

**Tiempo estimado:** 8 minutos

**Instrucciones:**

1. Con el documento completo abierto, ve al **panel lateral de Copilot**.

2. Escribe el siguiente prompt de validación:

   ```text
   Resume este documento en 5 puntos clave. Para cada punto, indica la sección del documento de donde proviene. Al final, identifica si hay alguna inconsistencia entre las secciones (por ejemplo, un competidor mencionado en el benchmarking pero no considerado en el análisis de brechas, o una tendencia sin conexión con las oportunidades).
   ```

3. Revisa el resumen generado por Copilot:
   - ¿Los 5 puntos clave capturan la esencia del informe?
   - ¿Copilot identificó alguna inconsistencia? Si es así, corrígela manualmente en el documento.

4. Ahora realiza una revisión de formato y estructura. Verifica que el documento contenga las siguientes secciones **en este orden**:

   | # | Sección | Formato esperado |
   |---|---|---|
   | 1 | Resumen Ejecutivo | Prosa, ~1 página |
   | 2 | Análisis de Tendencias del Mercado | Tabla (5 tendencias × 4 columnas) |
   | 3 | Benchmarking Competitivo | 2 tablas + 4 hallazgos |
   | 4 | Mapa de Posicionamiento Competitivo | Tabla de coordenadas + descripciones |
   | 5 | Análisis de Brechas y Oportunidades | 2 tablas + párrafo de síntesis |
   | 6 | Propuesta de Valor Diferenciada | Statement + 3 pilares + párrafo cierre |

5. Agrega un **título principal** al documento:
   - Coloca el cursor al inicio del documento (Ctrl + Inicio).
   - Presiona **Enter** para crear una línea nueva arriba.
   - Escribe: `Informe Ejecutivo de Posicionamiento — Marca Nexo`
   - Aplícale estilo **Título 1** desde la cinta de opciones.

6. Opcionalmente, agrega la fecha y el nombre del autor debajo del título en formato de texto normal.

7. Guarda el documento final con **Ctrl + S**.

8. Verifica que el nombre del archivo siga siendo `M1_Informe_Ejecutivo_Posicionamiento.docx` y que esté guardado en `Documentos/CopilotComunicacionEstrategia/M1_Informe_Ejecutivo/`.

**Resultado esperado:** Documento completo, coherente y con formato profesional que contiene 6 secciones estructuradas, un título principal y formato de encabezados consistente.

**Verificación:**
- El resumen de Copilot cubre las 6 secciones del documento.
- No hay inconsistencias evidentes entre secciones (competidores, tendencias y brechas están alineados).
- El documento tiene un título de nivel 1 y secciones con títulos de nivel 2.
- El archivo está guardado en la ruta correcta de OneDrive.

---

### Paso 8 — Generar una versión resumida para validación cruzada

**Objetivo:** Usar la función "Resumir este documento" de Copilot para crear un resumen ejecutivo de control que permita verificar la calidad global del informe.

**Tiempo estimado:** 5 minutos

**Instrucciones:**

1. En el **panel lateral de Copilot**, escribe:

   ```text
   Genera un resumen ejecutivo de este documento completo en exactamente 10 oraciones. Cada oración debe cubrir un hallazgo o recomendación diferente. Numera las oraciones.
   ```

2. Lee las 10 oraciones generadas. Evalúa:
   - ¿Cada oración aporta información diferente y no redundante?
   - ¿Las recomendaciones son coherentes con el análisis?
   - ¿Algún aspecto importante del informe quedó fuera del resumen?

3. Si el resumen revela que alguna sección del informe es débil o incompleta, regresa a esa sección y usa **"Borrador con Copilot"** o **"Reescribir con Copilot"** para fortalecerla.

4. **Copia las 10 oraciones del resumen** y pégalas al final del documento bajo un nuevo encabezado de nivel 2: `## Anexo: Resumen de Control (10 Puntos Clave)`.

5. Guarda con **Ctrl + S**.

**Resultado esperado:** Un anexo al final del documento con 10 oraciones numeradas que sintetizan todo el informe, sirviendo como herramienta de validación rápida.

**Verificación:**
- Las 10 oraciones están numeradas y son distintas entre sí.
- Al menos 1 oración referencia el benchmarking competitivo.
- Al menos 1 oración referencia la propuesta de valor.
- Al menos 1 oración referencia una oportunidad o brecha estratégica.

---

## Validación y Pruebas Finales

Antes de dar por completado el laboratorio, verifica los siguientes criterios de aceptación:

### Lista de Verificación del Entregable

| # | Criterio | ✅ / ❌ |
|---|---|---|
| 1 | La estructura de 4 carpetas existe en `Documentos/CopilotComunicacionEstrategia/` en OneDrive | |
| 2 | El archivo se llama exactamente `M1_Informe_Ejecutivo_Posicionamiento.docx` | |
| 3 | El archivo está guardado en `M1_Informe_Ejecutivo/` | |
| 4 | El documento tiene un título de nivel 1 (Título 1) al inicio | |
| 5 | Contiene sección "Resumen Ejecutivo" (~1 página, prosa profesional) | |
| 6 | Contiene sección "Análisis de Tendencias" con tabla de 5 tendencias | |
| 7 | Contiene sección "Benchmarking Competitivo" con al menos 3 competidores analizados | |
| 8 | Contiene matriz comparativa con al menos 5 criterios de evaluación | |
| 9 | Contiene sección "Mapa de Posicionamiento" con tabla de coordenadas | |
| 10 | Contiene sección "Análisis de Brechas y Oportunidades" con 2 tablas | |
| 11 | Contiene sección "Propuesta de Valor Diferenciada" con statement + 3 pilares | |
| 12 | Contiene "Anexo: Resumen de Control" con 10 puntos numerados | |
| 13 | Todos los encabezados usan estilos de Word consistentes (Título 1, 2, 3) | |
| 14 | No hay texto placeholder sin resolver (tipo "[INSERTAR AQUÍ]") | |
| 15 | El documento se sincronizó correctamente con OneDrive (verificar en onedrive.com) | |

### Prueba de Integridad para el Módulo 2

El documento generado en este laboratorio será referenciado por Copilot en el Módulo 2. Para asegurar la continuidad:

1. Abre **Microsoft Edge** → Navega a [onedrive.com](https://onedrive.com).
2. Busca el archivo `M1_Informe_Ejecutivo_Posicionamiento.docx` en la ruta esperada.
3. Ábrelo en Word Online y verifica que todo el contenido se visualiza correctamente.
4. Confirma que el archivo tiene un tamaño superior a 15 KB (un documento con 6 secciones completas debería pesar entre 20-80 KB).

---

## Solución de Problemas

### Problema 1: Copilot no aparece en la cinta de opciones de Word

**Síntomas:** Al abrir Word, no se ve el ícono de Copilot en la pestaña Inicio. La opción "Borrador con Copilot" no aparece al colocar el cursor en un documento vacío. El panel lateral de Copilot no está disponible.

**Causa:** La licencia de Microsoft Copilot for Microsoft 365 no está asignada a la cuenta del usuario, o la versión de Microsoft 365 Apps es anterior a la 2405 (Build 17628.20144), o Word no ha descargado la actualización que incluye Copilot.

**Solución:**
1. Verifica la licencia: Pide al administrador de TI que confirme en **admin.microsoft.com** → **Usuarios** → **Usuarios activos** → [tu cuenta] → **Licencias y aplicaciones** que "Microsoft Copilot for Microsoft 365" esté habilitado con la casilla marcada.
2. Verifica la versión: En Word, ve a **Archivo** → **Cuenta** → **Acerca de Word**. Si la versión es inferior a 2405, haz clic en **Opciones de actualización** → **Actualizar ahora**. Espera a que la actualización se complete y reinicia Word.
3. Si la licencia está asignada y la versión es correcta, cierra todas las aplicaciones de Office, espera 5 minutos (para que el servicio de licencias se sincronice) y vuelve a abrir Word.
4. Como último recurso, cierra sesión de tu cuenta Microsoft en Word (**Archivo** → **Cuenta** → **Cerrar sesión**), reinicia Word e inicia sesión nuevamente.

---

### Problema 2: Copilot genera contenido genérico que no refleja el caso de Marca Nexo

**Síntomas:** Al usar "Borrador con Copilot", la respuesta es un análisis genérico de la industria de bebidas sin mencionar a Marca Nexo, sin datos específicos del mercado mexicano, o con competidores de otros países o categorías. Las tablas no siguen el formato solicitado.

**Causa:** El prompt carece de suficiente contexto específico, las restricciones no fueron incluidas, o el prompt se truncó al ser demasiado largo para el campo de entrada. También puede ocurrir si el documento no tiene contenido previo que Copilot pueda usar como referencia (especialmente en los prompts de encadenamiento de los Pasos 4-6).

**Solución:**
1. **Verifica que el prompt completo fue ingresado:** Copilot en Word tiene un límite de caracteres en el campo de "Borrador con Copilot". Si tu prompt es muy largo, divídelo en dos partes: primero genera el contenido base y luego usa "Reescribir con Copilot" para añadir especificidad.
2. **Fortalece el contexto:** Asegúrate de que el prompt incluya explícitamente: nombre de la marca (Marca Nexo), país (México), categoría (bebidas funcionales), segmento (premium, ABC+) y canal (moderno). Si alguno de estos datos falta, Copilot generalizará.
3. **Para prompts de encadenamiento (Pasos 4-6):** Verifica que las secciones previas ya estén **conservadas** en el documento (no solo generadas en preview). Copilot solo puede referenciar contenido que ya forma parte del documento guardado. Si generaste contenido pero no hiciste clic en "Conservar", Copilot no lo ve.
4. **Regenera con ajustes:** Haz clic en "Regenerar" y añade al inicio del prompt: `"Importante: Toda la respuesta debe ser específica para Marca Nexo, una empresa mexicana de bebidas funcionales premium. No generes contenido genérico."` Esta instrucción explícita de restricción suele mejorar significativamente la especificidad.

---

## Limpieza del Entorno

Este laboratorio no requiere limpieza, ya que todos los archivos generados son insumos necesarios para los módulos posteriores del curso.

**No elimines:**
- La estructura de carpetas en `Documentos/CopilotComunicacionEstrategia/`
- El archivo `M1_Informe_Ejecutivo_Posicionamiento.docx`

**Acciones opcionales de orden:**
- Si durante el laboratorio creaste documentos de prueba o borradores adicionales, puedes eliminarlos para mantener limpia la carpeta `M1_Informe_Ejecutivo/`.
- Verifica que no haya archivos duplicados (por ejemplo, `M1_Informe_Ejecutivo_Posicionamiento (1).docx`). Si existen, conserva únicamente la versión final y elimina las copias.

---

## Resumen del Laboratorio

### Lo que lograste

En este laboratorio de 72 minutos:

1. **Creaste la infraestructura del curso:** Estructura de 4 carpetas en OneDrive que servirá como repositorio de trabajo para todos los módulos.

2. **Dominaste el marco RCTF:** Aplicaste Rol, Contexto, Tarea y Formato en múltiples prompts, comprobando cómo cada componente mejora la calidad de las respuestas de Copilot.

3. **Practicaste 3 técnicas avanzadas de prompting:**
   - **Restricciones** para acotar el alcance y evitar generalidades.
   - **Encadenamiento de prompts** para construir análisis complejos de forma progresiva.
   - **Iteración con "Reescribir con Copilot"** para refinar outputs específicos.

4. **Construiste un informe ejecutivo profesional** con 6 secciones estructuradas: resumen ejecutivo, tendencias, benchmarking, mapa de posicionamiento, brechas/oportunidades y propuesta de valor.

5. **Validaste la coherencia del documento** usando Copilot como herramienta de revisión y síntesis.

### Conexión con el Módulo 2

El archivo `M1_Informe_Ejecutivo_Posicionamiento.docx` será utilizado como contexto de referencia en el **Módulo 2: Estrategia Comercial y Precios**. Copilot podrá referenciar este documento para generar estrategias de pricing coherentes con el posicionamiento competitivo aquí definido. Asegúrate de que el archivo esté guardado y sincronizado en OneDrive antes de la siguiente sesión.

### Recursos Adicionales

| Recurso | Enlace |
|---|---|
| Introducción a Copilot para Microsoft 365 | [learn.microsoft.com](https://learn.microsoft.com/es-es/copilot/microsoft-365/microsoft-365-copilot-overview) |
| Técnicas de prompting de Microsoft | [learn.microsoft.com](https://learn.microsoft.com/es-es/azure/ai-services/openai/concepts/prompt-engineering) |
| Guía de mejores prácticas de prompts (OpenAI) | [platform.openai.com](https://platform.openai.com/docs/guides/prompt-engineering) |
| The economic potential of generative AI (McKinsey) | [mckinsey.com](https://www.mckinsey.com/capabilities/mckinsey-digital/our-insights/the-economic-potential-of-generative-ai-the-next-productivity-frontier) |

---
