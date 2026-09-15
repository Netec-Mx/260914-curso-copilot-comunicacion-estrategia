# Diseño de una matriz de estrategia comercial por canal y un plan piloto de precios adaptado a la competencia

## Metadatos

| Campo | Detalle |
|---|---|
| **Duración** | 96 minutos |
| **Complejidad** | Alta |
| **Nivel de Bloom** | Crear |
| **Módulo** | 2 — Estrategia Comercial y Precios |
| **Archivo entregable** | `M2_Estrategia_Comercial_Precios.xlsx` |

---

## Descripción General

En este laboratorio construirás desde cero un libro de Excel con cuatro hojas interconectadas que conforman una estrategia comercial completa para **Marca Nexo — línea de bebidas funcionales**. Utilizarás Microsoft Copilot en Excel para generar matrices de canal, definir el portafolio de productos, simular tres escenarios de precios y diseñar un plan piloto de 90 días. Todo el trabajo se apoya en los insights competitivos generados en el Módulo 1 (`M1_Informe_Ejecutivo_Posicionamiento.docx`), demostrando la continuidad del portafolio de trabajo construido a lo largo del curso.

---

## Objetivos de Aprendizaje

Al completar este laboratorio, serás capaz de:

- [ ] Construir una matriz de estrategia comercial multicanal en Excel con Copilot, definiendo roles, objetivos, métricas y tácticas para cuatro canales de distribución.
- [ ] Diseñar un modelo de simulación de escenarios de precios (conservador, base, agresivo) utilizando prompts de lenguaje natural en Copilot para generar fórmulas y lógica de cálculo.
- [ ] Aplicar ingeniería de prompts avanzada que referencie archivos previos del Módulo 1 como contexto, maximizando la relevancia y continuidad de los outputs.
- [ ] Producir un plan piloto de precios con cronograma de 90 días, métricas de éxito y criterios de escalamiento, listo para validación ejecutiva.
- [ ] Generar gráficos de análisis de escenarios y resúmenes narrativos directamente desde Copilot en Excel.

---

## Prerrequisitos

### Conocimientos previos

| Requisito | Nivel |
|---|---|
| Navegación en Microsoft Excel (hojas, celdas, tablas, formato) | Básico-Intermedio |
| Conceptos de canal de distribución (moderno, tradicional, e-commerce, directo) | Introductorio |
| Conceptos de margen comercial, precio de lista y precio al consumidor | Introductorio |
| Uso del panel lateral de Copilot en aplicaciones de Microsoft 365 | Completado en Módulo 1 |
| Ingeniería de prompts con contexto, datos y marco analítico | Completado en Módulo 1 |

### Acceso y archivos requeridos

| Elemento | Verificación |
|---|---|
| Licencia **Microsoft Copilot for Microsoft 365** asignada y activa | Confirmar en [admin.microsoft.com](https://admin.microsoft.com) o probar el ícono de Copilot en Excel |
| Microsoft 365 Apps versión **2405 (Build 17628.20144)** o superior | Excel → Archivo → Cuenta → Acerca de Excel |
| Archivo `M1_Informe_Ejecutivo_Posicionamiento.docx` disponible en OneDrive | Ruta: `Documentos/CopilotComunicacionEstrategia/M1_Informe_Ejecutivo/` |
| Carpeta `M2_Estrategia_Comercial` creada en OneDrive | Ruta: `Documentos/CopilotComunicacionEstrategia/M2_Estrategia_Comercial/` |
| Conexión a internet estable (mínimo 10 Mbps descarga / 5 Mbps subida) | Probar acceso a [office.com](https://office.com) |

> **⚠️ Nota sobre archivos semilla:** Si no completaste el Módulo 1, solicita al instructor el archivo semilla `M1_Informe_Ejecutivo_Posicionamiento.docx` antes de iniciar. Sin este archivo, los prompts con referencia cruzada no funcionarán correctamente.

---

## Entorno del Laboratorio

### Hardware mínimo

| Componente | Especificación |
|---|---|
| Procesador | Intel Core i5 8.ª gen. / AMD Ryzen 5 3000 o superior |
| RAM | 8 GB mínimo (16 GB recomendado) |
| Pantalla | 1366×768 mínimo (1920×1080 recomendado) |
| Almacenamiento | 10 GB disponibles (SSD recomendado) |
| Periféricos | Ratón externo recomendado para trabajo preciso en Excel |

### Software requerido

| Aplicación | Versión mínima |
|---|---|
| Microsoft Excel (Microsoft 365 Apps) | 2405 (Build 17628.20144) — Canal Mensual |
| Microsoft Word (Microsoft 365 Apps) | 2405 (Build 17628.20144) — Canal Mensual |
| Microsoft Copilot for Microsoft 365 | Release de servicio mayo 2024 o posterior |
| OneDrive for Business (cliente de sincronización) | 24.071.0407.0003 o superior |
| Microsoft Edge | 126.0.2592.68 o superior |

### Configuración inicial del entorno

Antes de iniciar los pasos del laboratorio, verifica lo siguiente:

1. Abre **Explorador de archivos** y navega a `OneDrive > Documentos > CopilotComunicacionEstrategia`.
2. Confirma que existe la subcarpeta `M1_Informe_Ejecutivo` con el archivo `M1_Informe_Ejecutivo_Posicionamiento.docx`.
3. Confirma que existe la subcarpeta `M2_Estrategia_Comercial`. Si no existe, créala ahora:
   - Clic derecho → **Nueva carpeta** → Nombre: `M2_Estrategia_Comercial`
4. Abre **Microsoft Excel** y confirma que el ícono de Copilot (✨) aparece en la cinta de opciones de la pestaña **Inicio**.
5. Si el ícono de Copilot no aparece, cierra Excel, verifica la versión en **Archivo → Cuenta → Acerca de Excel** y actualiza si es necesario.

---

## Instrucciones Paso a Paso

### Paso 1 — Crear el libro de Excel y la estructura de hojas (8 minutos)

**Objetivo:** Crear el archivo `M2_Estrategia_Comercial_Precios.xlsx` con las cuatro hojas de trabajo que conformarán la estrategia comercial completa.

**Instrucciones:**

1. Abre **Microsoft Excel** y selecciona **Libro en blanco**.

2. Guarda inmediatamente el archivo:
   - **Archivo → Guardar como → OneDrive**
   - Navega a: `Documentos/CopilotComunicacionEstrategia/M2_Estrategia_Comercial/`
   - Nombre del archivo: `M2_Estrategia_Comercial_Precios.xlsx`
   - Haz clic en **Guardar**.

3. Renombra la primera hoja (pestaña inferior):
   - Doble clic en la pestaña `Hoja1` → escribe `Matriz_Canales` → presiona **Enter**.

4. Crea la segunda hoja:
   - Haz clic en el ícono **+** junto a la pestaña → renómbrala como `Portafolio_Productos`.

5. Crea la tercera hoja:
   - Haz clic en **+** → renómbrala como `Simulacion_Precios`.

6. Crea la cuarta hoja:
   - Haz clic en **+** → renómbrala como `Plan_Piloto`.

7. Guarda el archivo con **Ctrl + S**.

**Resultado esperado:** Un libro de Excel guardado en la ruta correcta de OneDrive con cuatro hojas nombradas: `Matriz_Canales`, `Portafolio_Productos`, `Simulacion_Precios` y `Plan_Piloto`.

**Verificación:**
- Las cuatro pestañas son visibles en la parte inferior de Excel.
- La barra de título muestra `M2_Estrategia_Comercial_Precios.xlsx` con el ícono de nube de OneDrive (sincronizado).
- El ícono de Copilot (✨) está visible en la cinta de opciones.

---

### Paso 2 — Extraer insights del Módulo 1 con Copilot en Word (10 minutos)

**Objetivo:** Abrir el informe ejecutivo del Módulo 1 y usar Copilot para extraer un resumen de insights competitivos que servirá como contexto para los prompts en Excel.

**Instrucciones:**

1. Abre **Microsoft Word** (sin cerrar Excel).

2. Abre el archivo `M1_Informe_Ejecutivo_Posicionamiento.docx` desde:
   `OneDrive > Documentos > CopilotComunicacionEstrategia > M1_Informe_Ejecutivo`

3. Haz clic en el ícono de **Copilot** (✨) en la cinta de opciones de Word para abrir el panel lateral de Copilot.

4. En el panel lateral de Copilot, escribe el siguiente prompt:

```text
Resume en formato de lista con viñetas los siguientes elementos extraídos de este documento:
1. Los 3-5 principales competidores de Marca Nexo identificados
2. Las ventajas competitivas clave de Marca Nexo
3. Las brechas o debilidades detectadas en el posicionamiento
4. Los segmentos de mercado con mayor oportunidad
5. Los rangos de precios observados en la competencia

Sé específico con datos y cifras cuando estén disponibles. Formatea la respuesta para que pueda copiarse fácilmente.
```

5. Revisa la respuesta de Copilot. Si el documento del Módulo 1 contiene datos cuantitativos, estos deben aparecer en el resumen.

6. **Copia la respuesta completa** de Copilot:
   - Haz clic en el ícono de **copiar** (📋) en la respuesta de Copilot, o selecciona todo el texto y presiona **Ctrl + C**.

7. Abre un archivo temporal de notas o pega el contenido en un **Bloc de notas** para tenerlo disponible durante el resto del laboratorio:
   - Abre Bloc de notas (Windows + R → `notepad` → Enter).
   - Pega con **Ctrl + V**.
   - Guarda como `Notas_Insights_M1.txt` en la carpeta `M2_Estrategia_Comercial`.

> **💡 Consejo:** Este resumen de insights será el "contexto de negocio" que incluirás en cada prompt de Copilot en Excel. Tenerlo accesible evita que tengas que alternar constantemente entre Word y Excel.

**Resultado esperado:** Un resumen estructurado en viñetas con los insights competitivos clave de Marca Nexo, guardado en un archivo de texto accesible.

**Verificación:**
- El resumen contiene al menos 3 competidores identificados.
- Incluye información sobre rangos de precios competitivos.
- Menciona segmentos de mercado y oportunidades.
- El archivo `Notas_Insights_M1.txt` está guardado en la carpeta `M2_Estrategia_Comercial`.

---

### Paso 3 — Construir la Matriz de Canales con Copilot en Excel (18 minutos)

**Objetivo:** Crear una tabla estructurada en la hoja `Matriz_Canales` que defina la estrategia comercial para cada canal de distribución, utilizando Copilot para generar la estructura y el contenido estratégico.

**Instrucciones:**

1. Regresa a **Excel** y haz clic en la pestaña `Matriz_Canales`.

2. Haz clic en la celda **A1** y escribe el encabezado: `MATRIZ DE ESTRATEGIA COMERCIAL POR CANAL — MARCA NEXO`. Aplica formato **Negrita** y tamaño de fuente **14**.

3. En la celda **A3**, escribe los siguientes encabezados de columna (uno por celda, de A3 a H3):

| Celda | Encabezado |
|---|---|
| A3 | Canal |
| B3 | Rol Estratégico |
| C3 | Segmento Objetivo |
| D3 | Propuesta de Valor por Canal |
| E3 | KPIs Clave |
| F3 | Tácticas Recomendadas |
| G3 | Prioridad (Alta/Media/Baja) |
| H3 | Presupuesto Relativo (%) |

4. En las celdas **A4 a A7**, escribe los cuatro canales:
   - A4: `Canal Moderno (Supermercados)`
   - A5: `Canal Tradicional (Tiendas de barrio)`
   - A6: `E-commerce`
   - A7: `Canal Directo (Venta propia)`

5. Selecciona el rango **A3:H7** (encabezados + filas de canales).

6. Convierte el rango en **Tabla de Excel**:
   - Ve a **Insertar → Tabla** (o presiona **Ctrl + T**).
   - Confirma que "La tabla tiene encabezados" esté marcado.
   - Haz clic en **Aceptar**.

> **⚠️ Importante:** Copilot en Excel funciona óptimamente con datos formateados como **Tablas de Excel** (no rangos simples). Este paso es indispensable para que los prompts posteriores funcionen correctamente.

7. Con la tabla seleccionada, haz clic en el ícono de **Copilot** (✨) en la cinta de opciones para abrir el panel lateral.

8. En el panel de Copilot, escribe el siguiente prompt. **Antes de enviarlo**, reemplaza `[PEGAR INSIGHTS]` con el resumen que copiaste en el Paso 2:

```text
Tengo una tabla con la estrategia comercial por canal para Marca Nexo, una línea de bebidas funcionales (energía, hidratación, bienestar) dirigida al mercado latinoamericano.

Contexto competitivo del Módulo 1:
[PEGAR INSIGHTS DEL ARCHIVO M1 AQUÍ]

Completa las columnas vacías de la tabla para cada canal con la siguiente lógica:
- Rol Estratégico: Define si el canal es de penetración/volumen, rentabilidad, construcción de marca o experimentación.
- Segmento Objetivo: Identifica el perfil demográfico y psicográfico principal que compra en ese canal.
- Propuesta de Valor por Canal: Qué mensaje o beneficio resaltar en ese punto de contacto.
- KPIs Clave: 3 indicadores medibles para evaluar el desempeño en ese canal.
- Tácticas Recomendadas: 2-3 acciones concretas (promociones, exhibición, bundles, sampling, etc.)
- Prioridad: Alta, Media o Baja según el potencial de retorno.
- Presupuesto Relativo: Porcentaje sugerido del presupuesto comercial total (los 4 canales deben sumar 100%).
```

9. Revisa la respuesta de Copilot. Copilot puede:
   - Sugerir completar las celdas directamente en la tabla, o
   - Proporcionar el contenido en formato texto para que lo copies manualmente.

10. Si Copilot genera el contenido como texto, **copia cada celda manualmente** a la tabla. Si ofrece la opción de insertar directamente, haz clic en **Insertar** o **Aplicar**.

11. **Refinamiento:** Si alguna celda tiene contenido genérico o poco específico para bebidas funcionales, envía un prompt de seguimiento:

```text
La celda de Tácticas Recomendadas para el canal E-commerce es demasiado genérica. 
Reescríbela con tácticas específicas para una marca de bebidas funcionales que compite 
con [nombre de competidor del M1] en marketplaces como MercadoLibre y Amazon. 
Incluye tácticas de suscripción, bundles de variedad y colaboraciones con influencers de bienestar.
```

12. Ajusta el ancho de las columnas para que todo el contenido sea legible:
    - Selecciona todas las columnas (clic en el selector de esquina superior izquierda).
    - **Formato → Ancho de columna automático** o doble clic en el borde de cualquier encabezado de columna.

13. Aplica formato visual a la tabla:
    - Haz clic en cualquier celda de la tabla.
    - Ve a **Diseño de tabla** (pestaña contextual) → selecciona un estilo de tabla con colores corporativos (recomendado: tonos azules o verdes).

14. Guarda con **Ctrl + S**.

**Resultado esperado:** Una tabla completa de 4 filas × 8 columnas con estrategia diferenciada por canal. Los porcentajes de presupuesto suman 100%. Cada canal tiene KPIs específicos y tácticas accionables.

**Verificación:**
- [ ] Las cuatro filas de canales tienen todas las columnas completadas.
- [ ] Los porcentajes de la columna `Presupuesto Relativo (%)` suman 100%.
- [ ] Los KPIs son medibles (contienen métricas como "sell-out mensual", "tasa de conversión", "cobertura numérica", etc.).
- [ ] Las tácticas son específicas para bebidas funcionales (no genéricas).
- [ ] La tabla está formateada como Tabla de Excel (visible en la pestaña contextual "Diseño de tabla").

---

### Paso 4 — Definir el Portafolio de Productos con Copilot (15 minutos)

**Objetivo:** Crear en la hoja `Portafolio_Productos` una tabla que defina los SKUs de Marca Nexo con atributos estratégicos, clasificación BCG y canal preferente.

**Instrucciones:**

1. Haz clic en la pestaña `Portafolio_Productos`.

2. En la celda **A1**, escribe: `PORTAFOLIO DE PRODUCTOS — MARCA NEXO` (Negrita, tamaño 14).

3. Haz clic en el ícono de **Copilot** (✨) en la cinta de opciones.

4. En el panel de Copilot, escribe el siguiente prompt:

```text
Actúa como consultor de estrategia de portafolio para Marca Nexo, una línea de bebidas funcionales con tres categorías: Energía, Hidratación y Bienestar.

Crea una tabla de portafolio de productos con 8 SKUs distribuidos entre las tres categorías. 
Usa los siguientes encabezados de columna:
- SKU (código alfanumérico)
- Nombre del Producto
- Categoría (Energía / Hidratación / Bienestar)
- Presentación (ml)
- Precio de Lista Sugerido (USD)
- Margen Bruto Estimado (%)
- Etapa del Ciclo de Vida (Lanzamiento / Crecimiento / Madurez / Declive)
- Clasificación BCG (Estrella / Vaca / Interrogante / Perro)
- Rol de Portafolio (Entrada / Volumen / Rentabilidad / Imagen)
- Canal Preferente (Moderno / Tradicional / E-commerce / Directo)
- Prioridad Comercial (1-Alta, 2-Media, 3-Baja)

Criterios para los datos:
- Los precios deben estar entre USD 1.50 y USD 4.50
- Los márgenes entre 25% y 55%
- Debe haber al menos un producto en cada clasificación BCG
- Los productos de Imagen deben tener precio premium y margen alto
- Los productos de Entrada deben tener precio accesible

Genera la tabla completa con datos realistas para el mercado latinoamericano de bebidas funcionales.
```

5. Cuando Copilot genere la respuesta:
   - Si ofrece insertar la tabla directamente, haz clic en **Insertar**.
   - Si genera texto, copia los datos y pégalos a partir de la celda **A3**.

6. **Convierte el rango en Tabla de Excel:**
   - Selecciona todo el rango de datos (encabezados + 8 filas de productos).
   - **Ctrl + T** → Confirma encabezados → **Aceptar**.

7. Valida la coherencia de los datos con un prompt de seguimiento:

```text
Revisa la tabla de portafolio que acabamos de crear. Verifica que:
1. Hay al menos un producto en cada clasificación BCG
2. Los precios de los productos de "Entrada" son los más bajos
3. Los productos de "Imagen" tienen el margen más alto
4. La asignación de canal preferente es coherente con el rol de portafolio
Si encuentras inconsistencias, sugiere los ajustes específicos.
```

8. Aplica los ajustes sugeridos por Copilot manualmente si es necesario.

9. Agrega una fila de **totales/promedios** debajo de la tabla:
   - En la celda debajo de `Precio de Lista Sugerido`, escribe: `=AVERAGE(` y selecciona la columna de precios `)`.
   - Repite para `Margen Bruto Estimado`.

10. Aplica formato condicional a la columna `Prioridad Comercial`:
    - Selecciona la columna de prioridad.
    - **Inicio → Formato condicional → Escalas de color** → selecciona una escala de verde (alta) a rojo (baja).

11. Guarda con **Ctrl + S**.

**Resultado esperado:** Una tabla de 8 SKUs con 11 columnas completamente pobladas, datos coherentes entre clasificación BCG, rol de portafolio y canal preferente, con formato condicional aplicado.

**Verificación:**
- [ ] Hay exactamente 8 productos distribuidos en 3 categorías.
- [ ] Cada clasificación BCG tiene al menos un producto.
- [ ] Los precios están en el rango USD 1.50–4.50.
- [ ] Los márgenes están en el rango 25%–55%.
- [ ] El formato condicional de prioridad es visible.
- [ ] Los datos están en formato de Tabla de Excel.

---

### Paso 5 — Construir el modelo de simulación de precios con Copilot (22 minutos)

**Objetivo:** Crear en la hoja `Simulacion_Precios` un modelo de tres escenarios de precios (conservador, base, agresivo) con fórmulas generadas por Copilot, análisis de sensibilidad y gráfico comparativo.

**Instrucciones:**

#### Parte A — Estructura del modelo (8 minutos)

1. Haz clic en la pestaña `Simulacion_Precios`.

2. En la celda **A1**, escribe: `SIMULACIÓN DE ESCENARIOS DE PRECIOS — MARCA NEXO` (Negrita, tamaño 14).

3. En la celda **A3**, escribe: `Variables del Modelo` (Negrita).

4. Crea la siguiente tabla de variables a partir de la celda **A4**:

| Celda | Contenido | Celda | Valor |
|---|---|---|---|
| A4 | `Costo unitario promedio (USD)` | B4 | `1.20` |
| A5 | `Precio competidor líder (USD)` | B5 | `2.80` |
| A6 | `Precio competidor bajo (USD)` | B6 | `1.80` |
| A7 | `Volumen mensual estimado (unidades)` | B7 | `50000` |
| A8 | `Descuento canal moderno (%)` | B8 | `15` |
| A9 | `Descuento canal tradicional (%)` | B9 | `10` |
| A10 | `Descuento e-commerce (%)` | B10 | `20` |
| A11 | `Descuento canal directo (%)` | B11 | `5` |

> **💡 Nota:** Si tu informe del Módulo 1 contiene datos de precios competitivos específicos, reemplaza los valores de B5 y B6 con esos datos para mayor realismo.

5. Selecciona el rango **A4:B11** y conviértelo en Tabla de Excel (**Ctrl + T**). Nómbrala `Variables` (en **Diseño de tabla → Nombre de la tabla**).

#### Parte B — Tabla de escenarios con fórmulas generadas por Copilot (14 minutos)

6. En la celda **D3**, escribe: `Escenarios de Precios` (Negrita).

7. Crea los encabezados a partir de **D4**:

| Celda | Encabezado |
|---|---|
| D4 | `Métrica` |
| E4 | `Conservador` |
| F4 | `Base` |
| G4 | `Agresivo` |

8. En las celdas **D5 a D16**, escribe las siguientes métricas (una por fila):

```
Precio de lista (USD)
Precio al consumidor canal moderno (USD)
Precio al consumidor canal tradicional (USD)
Precio al consumidor e-commerce (USD)
Precio al consumidor canal directo (USD)
Margen bruto unitario (USD)
Margen bruto (%)
Ingreso mensual estimado (USD)
Costo total mensual (USD)
Utilidad bruta mensual (USD)
Índice vs. competidor líder (%)
Índice vs. competidor bajo (%)
```

9. Selecciona el rango **D4:G16** y conviértelo en Tabla de Excel (**Ctrl + T**). Nómbrala `Escenarios`.

10. Haz clic en el ícono de **Copilot** (✨) y escribe el siguiente prompt:

```text
Tengo dos tablas en esta hoja:
- Tabla "Variables" con costo unitario, precios de competidores, volumen mensual y descuentos por canal.
- Tabla "Escenarios" con filas de métricas y tres columnas de escenarios (Conservador, Base, Agresivo).

Genera las fórmulas para completar la tabla "Escenarios" con esta lógica:

PRECIOS DE LISTA:
- Conservador: 10% por debajo del competidor líder
- Base: 5% por debajo del competidor líder  
- Agresivo: igual al competidor líder

PRECIO AL CONSUMIDOR POR CANAL: Precio de lista × (1 - descuento del canal correspondiente de la tabla Variables)

MARGEN BRUTO UNITARIO: Precio de lista - Costo unitario promedio

MARGEN BRUTO (%): (Margen bruto unitario / Precio de lista) × 100

INGRESO MENSUAL: Precio de lista × Volumen mensual estimado

COSTO TOTAL MENSUAL: Costo unitario promedio × Volumen mensual estimado

UTILIDAD BRUTA MENSUAL: Ingreso mensual - Costo total mensual

ÍNDICE VS COMPETIDOR LÍDER: (Precio de lista / Precio competidor líder) × 100

ÍNDICE VS COMPETIDOR BAJO: (Precio de lista / Precio competidor bajo) × 100

Todas las fórmulas deben referenciar las celdas de la tabla "Variables" para que al cambiar un valor se actualicen automáticamente todos los escenarios.

Proporciona cada fórmula indicando la celda exacta donde debe ir.
```

11. Copilot generará las fórmulas. Aplica cada fórmula en la celda correspondiente. Ejemplo de fórmulas esperadas:

   - **E5** (Precio de lista Conservador): `=B5*(1-0.10)` → resultado: `2.52`
   - **F5** (Precio de lista Base): `=B5*(1-0.05)` → resultado: `2.66`
   - **G5** (Precio de lista Agresivo): `=B5` → resultado: `2.80`
   - **E6** (Precio consumidor canal moderno, Conservador): `=E5*(1-B8/100)`

> **⚠️ Importante:** Si Copilot genera fórmulas con referencias a nombres de tabla estructurada (ej. `Variables[Valor]`), estas son igualmente válidas. Lo esencial es que las fórmulas referencien la tabla de Variables y no contengan valores fijos ("hardcoded").

12. Una vez ingresadas todas las fórmulas, verifica la coherencia:
    - El margen bruto del escenario Agresivo debe ser el más alto.
    - Los índices vs. competidor líder deben ser: Conservador ≈ 90%, Base ≈ 95%, Agresivo ≈ 100%.
    - La utilidad bruta mensual debe ser positiva en los tres escenarios.

13. Aplica formato de número a las celdas:
    - Celdas de precios y montos: **Formato de número → Moneda (USD)** con 2 decimales.
    - Celdas de porcentaje: **Formato de número → Porcentaje** con 1 decimal.

14. Solicita a Copilot un gráfico comparativo:

```text
Crea un gráfico de barras agrupadas que compare los tres escenarios 
(Conservador, Base, Agresivo) para las siguientes métricas:
- Precio de lista
- Margen bruto (%)
- Utilidad bruta mensual

El gráfico debe tener título "Comparativo de Escenarios de Precios — Marca Nexo" 
y leyenda clara para cada escenario.
```

15. Si Copilot genera el gráfico, ajústalo de tamaño y posición. Si no puede generarlo directamente, créalo manualmente:
    - Selecciona las celdas de las tres métricas solicitadas para los tres escenarios.
    - **Insertar → Gráfico → Barras agrupadas**.
    - Agrega título y leyenda.

16. Posiciona el gráfico debajo de las tablas (aproximadamente a partir de la fila 20).

17. Guarda con **Ctrl + S**.

**Resultado esperado:** Un modelo de simulación con tabla de variables (editable), tabla de tres escenarios con fórmulas dinámicas y un gráfico comparativo. Al cambiar cualquier valor en la tabla de Variables, todos los escenarios se recalculan automáticamente.

**Verificación:**
- [ ] Cambia el valor de `Costo unitario promedio` de `1.20` a `1.40` y verifica que todas las fórmulas de margen y utilidad se actualizan automáticamente. **Regresa el valor a `1.20` después de verificar.**
- [ ] Los tres escenarios muestran utilidad bruta mensual positiva.
- [ ] Los índices de precio vs. competidores son coherentes (Conservador < Base < Agresivo).
- [ ] El gráfico refleja correctamente los datos de la tabla de escenarios.
- [ ] No hay fórmulas con valores fijos; todas referencian la tabla de Variables.

---

### Paso 6 — Análisis de sensibilidad con Copilot (10 minutos)

**Objetivo:** Agregar un análisis de sensibilidad que muestre cómo varía la utilidad bruta mensual al modificar el costo unitario y el volumen de ventas, utilizando Copilot para generar la estructura.

**Instrucciones:**

1. Posiciona el cursor en la celda **D20** (o debajo del gráfico si ocupa más espacio).

2. Escribe: `ANÁLISIS DE SENSIBILIDAD` (Negrita, tamaño 12).

3. Abre el panel de Copilot y escribe:

```text
Necesito crear una tabla de sensibilidad (tabla de datos de dos variables) que muestre 
la Utilidad Bruta Mensual del escenario BASE variando dos factores:

- Eje vertical (filas): Costo unitario promedio variando de 0.80 a 1.60 en incrementos de 0.10
- Eje horizontal (columnas): Volumen mensual variando de 30,000 a 70,000 en incrementos de 10,000

La celda de resultado debe referenciar la fórmula de Utilidad Bruta Mensual del escenario Base.

Indícame:
1. Cómo estructurar la tabla de datos
2. Las fórmulas o valores que debo colocar en cada celda de encabezado
3. Cómo usar la función "Tabla de datos" de Excel (Datos → Análisis de hipótesis → Tabla de datos) para llenar automáticamente los resultados
```

4. Sigue las instrucciones de Copilot para crear la tabla de sensibilidad. La estructura general será:

   - Celda de esquina (ej. D22): referencia a la fórmula de utilidad bruta mensual del escenario Base.
   - Fila superior (E22:I22): valores de volumen (30000, 40000, 50000, 60000, 70000).
   - Columna izquierda (D23:D31): valores de costo unitario (0.80, 0.90, 1.00, ..., 1.60).

5. Ejecuta la función **Tabla de datos**:
   - Selecciona todo el rango de la tabla de sensibilidad (incluyendo encabezados y celda de esquina).
   - Ve a **Datos → Análisis de hipótesis → Tabla de datos**.
   - **Celda de entrada de fila:** selecciona la celda B7 (Volumen mensual).
   - **Celda de entrada de columna:** selecciona la celda B4 (Costo unitario).
   - Haz clic en **Aceptar**.

6. Aplica formato condicional a los resultados:
   - Selecciona las celdas de resultados de la tabla de sensibilidad.
   - **Inicio → Formato condicional → Escalas de color** → selecciona verde (valores altos) a rojo (valores bajos).

7. Guarda con **Ctrl + S**.

**Resultado esperado:** Una tabla de sensibilidad de 9 filas × 5 columnas con valores de utilidad bruta calculados automáticamente, con formato condicional que permite identificar visualmente las combinaciones más y menos rentables.

**Verificación:**
- [ ] La tabla de sensibilidad muestra valores numéricos (no errores `#¡REF!` o `#¡VALOR!`).
- [ ] Los valores más altos (verde) corresponden a costo bajo + volumen alto.
- [ ] Los valores más bajos (rojo) corresponden a costo alto + volumen bajo.
- [ ] El valor en la intersección de costo 1.20 y volumen 50,000 coincide con la utilidad bruta del escenario Base en la tabla de escenarios.

---

### Paso 7 — Diseñar el Plan Piloto de Precios (13 minutos)

**Objetivo:** Crear en la hoja `Plan_Piloto` un plan de implementación de 90 días para probar la estrategia de precios del escenario seleccionado en un canal y segmento específicos.

**Instrucciones:**

1. Haz clic en la pestaña `Plan_Piloto`.

2. En la celda **A1**, escribe: `PLAN PILOTO DE PRECIOS — MARCA NEXO` (Negrita, tamaño 14).

3. En **A2**, escribe: `Escenario seleccionado: Base | Canal: Moderno (Supermercados) | Duración: 90 días`.

4. Abre el panel de Copilot y escribe el siguiente prompt:

```text
Diseña un plan piloto de precios para Marca Nexo (bebidas funcionales) con las siguientes especificaciones:

CONTEXTO:
- Se implementará el escenario de precios "Base" (precio de lista ~USD 2.66)
- Canal seleccionado: Canal Moderno (Supermercados)
- Duración: 90 días (3 fases de 30 días)
- Mercado piloto: 2 ciudades principales

Crea DOS tablas:

TABLA 1 — CRONOGRAMA DEL PILOTO (formato Gantt simplificado):
Columnas: Fase | Período | Actividad | Responsable | Entregable | Estado
- Fase 1 (Días 1-30): Preparación y lanzamiento
- Fase 2 (Días 31-60): Ejecución y monitoreo
- Fase 3 (Días 61-90): Evaluación y decisión de escalamiento
Incluye al menos 3 actividades por fase.

TABLA 2 — MÉTRICAS DE ÉXITO Y CRITERIOS DE ESCALAMIENTO:
Columnas: Métrica | Definición | Meta Mínima (Go) | Meta Objetivo | Umbral de Alerta (No-Go) | Frecuencia de Medición
Incluye al menos 6 métricas: sell-out, participación de mercado, margen realizado, cobertura de PDV, rotación de inventario, Net Promoter Score.

Genera datos realistas para el mercado latinoamericano de bebidas.
```

5. Cuando Copilot genere las tablas, insértalas en la hoja:
   - **Tabla 1** a partir de la celda **A4**.
   - **Tabla 2** a partir de la celda **A20** (o debajo de la Tabla 1 con 2 filas de separación).

6. Convierte ambos rangos en Tablas de Excel (**Ctrl + T**):
   - Tabla 1: nombre `Cronograma_Piloto`
   - Tabla 2: nombre `Metricas_Exito`

7. Agrega una sección de **Criterios de Escalamiento** debajo de la Tabla 2. Usa Copilot:

```text
Debajo de la tabla de métricas, agrega una sección de texto con el título 
"Criterios de Decisión Post-Piloto" que defina:

1. ESCALAR (Go): Condiciones específicas que deben cumplirse para expandir 
   el piloto a nivel nacional (ej. "Si X de Y métricas alcanzan la meta mínima...")
2. AJUSTAR: Condiciones para modificar el precio o las tácticas y extender 
   el piloto 30 días adicionales
3. CANCELAR (No-Go): Condiciones para detener el piloto y reevaluar la estrategia

Sé específico con umbrales numéricos basados en las métricas de la tabla anterior.
```

8. Copia el texto generado por Copilot y pégalo en las celdas correspondientes (a partir de la fila debajo de la Tabla 2). Usa **Combinar y centrar** para las celdas de texto largo si es necesario.

9. Aplica formato visual consistente:
   - Tabla 1: estilo de tabla con colores azules.
   - Tabla 2: estilo de tabla con colores verdes.
   - Sección de criterios: fondo amarillo claro para destacar.

10. En la columna `Estado` de la Tabla 1, agrega una lista desplegable de validación de datos:
    - Selecciona las celdas de la columna `Estado`.
    - **Datos → Validación de datos → Lista** → Origen: `Pendiente,En progreso,Completado,Bloqueado`
    - Haz clic en **Aceptar**.
    - Selecciona `Pendiente` como valor predeterminado en todas las celdas.

11. Guarda con **Ctrl + S**.

**Resultado esperado:** Un plan piloto estructurado con cronograma de 3 fases, al menos 9 actividades, 6+ métricas de éxito con umbrales claros, y criterios de decisión post-piloto.

**Verificación:**
- [ ] La Tabla 1 tiene al menos 9 filas (3 actividades × 3 fases).
- [ ] La Tabla 2 tiene al menos 6 métricas con todas las columnas completadas.
- [ ] Los criterios de escalamiento referencian métricas específicas de la Tabla 2.
- [ ] La lista desplegable de `Estado` funciona correctamente.
- [ ] Ambas tablas están formateadas como Tablas de Excel.

---

### Paso 8 — Generar resumen narrativo y validación final (Copilot) (Últimos minutos disponibles)

**Objetivo:** Usar Copilot para generar un resumen ejecutivo narrativo del modelo completo y realizar una validación cruzada entre las cuatro hojas.

**Instrucciones:**

1. Regresa a la hoja `Matriz_Canales`.

2. Abre el panel de Copilot y escribe:

```text
Analiza los datos de esta hoja y genera un resumen ejecutivo de 3-4 párrafos que explique:
1. Cuál es la estrategia de distribución de Marca Nexo por canal
2. Qué canal tiene la mayor prioridad y por qué
3. Cómo se distribuye el presupuesto comercial entre canales
4. Qué riesgos o dependencias deberían considerarse

Redacta en tono ejecutivo, como si fuera para presentar ante un comité directivo.
```

3. Copia el resumen generado.

4. Crea una **nueva hoja** en el libro: haz clic en **+** → renómbrala como `Resumen_Ejecutivo`.

5. Pega el resumen en la celda **A1** de la nueva hoja.

6. Navega a la hoja `Simulacion_Precios` y solicita a Copilot:

```text
Basándote en la tabla de escenarios de precios, responde:
1. ¿Cuál escenario ofrece el mejor balance entre competitividad y rentabilidad?
2. ¿Cuál es el riesgo principal del escenario agresivo?
3. ¿Qué variable tiene mayor impacto en la utilidad según la tabla de sensibilidad?

Resume en formato de bullet points ejecutivos.
```

7. Copia la respuesta y pégala en la hoja `Resumen_Ejecutivo` debajo del primer resumen.

8. Aplica formato al resumen:
   - Título: `RESUMEN EJECUTIVO — ESTRATEGIA COMERCIAL Y PRECIOS` (Negrita, tamaño 14).
   - Subtítulos para cada sección.
   - Fuente Calibri 11 para el cuerpo.

9. **Validación cruzada final:** Verifica manualmente que:
   - Los canales mencionados en `Matriz_Canales` coinciden con los canales de descuento en `Simulacion_Precios`.
   - Los productos de la hoja `Portafolio_Productos` son coherentes con el canal piloto seleccionado en `Plan_Piloto`.
   - El escenario seleccionado en `Plan_Piloto` corresponde a uno de los tres escenarios de `Simulacion_Precios`.

10. Guarda la versión final con **Ctrl + S**.

11. Verifica que el archivo esté sincronizado con OneDrive (ícono de nube con marca de verificación en la barra de título).

**Resultado esperado:** Un libro de Excel con 5 hojas (`Matriz_Canales`, `Portafolio_Productos`, `Simulacion_Precios`, `Plan_Piloto`, `Resumen_Ejecutivo`) que constituye una estrategia comercial completa y coherente.

**Verificación:**
- [ ] El archivo tiene 5 hojas con los nombres correctos.
- [ ] El resumen ejecutivo es coherente con los datos de las demás hojas.
- [ ] No hay errores de fórmula (#¡REF!, #¡VALOR!, #N/A) en ninguna hoja.
- [ ] El archivo está guardado como `M2_Estrategia_Comercial_Precios.xlsx` en la ruta correcta de OneDrive.

---

## Validación y Pruebas

Antes de considerar el laboratorio completado, ejecuta la siguiente lista de validación integral:

### Validación de estructura

| # | Criterio | ✅/❌ |
|---|---|---|
| 1 | El archivo se llama exactamente `M2_Estrategia_Comercial_Precios.xlsx` | |
| 2 | Está guardado en `OneDrive/Documentos/CopilotComunicacionEstrategia/M2_Estrategia_Comercial/` | |
| 3 | Contiene 5 hojas: `Matriz_Canales`, `Portafolio_Productos`, `Simulacion_Precios`, `Plan_Piloto`, `Resumen_Ejecutivo` | |
| 4 | Todas las tablas de datos están formateadas como **Tablas de Excel** (no rangos simples) | |

### Validación de contenido

| # | Criterio | ✅/❌ |
|---|---|---|
| 5 | `Matriz_Canales`: 4 canales × 8 columnas, completamente poblada | |
| 6 | `Portafolio_Productos`: 8 SKUs con 11 atributos, clasificación BCG coherente | |
| 7 | `Simulacion_Precios`: 3 escenarios con fórmulas dinámicas (no valores fijos) | |
| 8 | `Simulacion_Precios`: Tabla de sensibilidad funcional con formato condicional | |
| 9 | `Simulacion_Precios`: Gráfico comparativo de escenarios presente | |
| 10 | `Plan_Piloto`: Cronograma de 3 fases con 9+ actividades | |
| 11 | `Plan_Piloto`: 6+ métricas de éxito con umbrales Go/No-Go | |
| 12 | `Resumen_Ejecutivo`: Narrativa coherente con datos de las demás hojas | |

### Validación de funcionalidad

| # | Criterio | ✅/❌ |
|---|---|---|
| 13 | Al cambiar el costo unitario en la tabla Variables, todos los escenarios se recalculan | |
| 14 | Al cambiar el volumen mensual, los ingresos y utilidades se actualizan | |
| 15 | La lista desplegable de `Estado` en el Plan Piloto funciona correctamente | |
| 16 | Los porcentajes de presupuesto en Matriz_Canales suman 100% | |

---

## Solución de Problemas

### Problema 1: Copilot no genera fórmulas ni analiza datos en Excel

**Síntomas:** Al abrir el panel de Copilot en Excel y escribir un prompt que solicita fórmulas o análisis de datos, Copilot responde con texto genérico, indica que no puede acceder a los datos, o muestra el mensaje "No puedo ayudarte con eso en este momento".

**Causa:** Copilot en Excel requiere que los datos estén formateados como **Tabla de Excel** (objeto de tabla, no rango simple). Además, el archivo debe estar guardado en **OneDrive o SharePoint** (no en disco local) y la función de autoguardado debe estar activada. Si alguna de estas condiciones no se cumple, Copilot no puede interactuar con los datos de la hoja.

**Solución:**
1. Verifica que los datos están en formato de Tabla de Excel: haz clic en cualquier celda con datos → si la pestaña contextual **"Diseño de tabla"** aparece en la cinta, es una tabla. Si no aparece, selecciona el rango y presiona **Ctrl + T** para convertirlo.
2. Verifica que el archivo está en OneDrive: la barra de título debe mostrar el ícono de nube. Si dice "Este equipo" o muestra una ruta local, ve a **Archivo → Guardar como → OneDrive** y guárdalo en la ruta del laboratorio.
3. Activa el **Autoguardado**: el interruptor de Autoguardado en la esquina superior izquierda de Excel debe estar en **Activado** (verde). Si está desactivado, actívalo y selecciona la ubicación de OneDrive cuando se solicite.
4. Cierra y reabre el panel de Copilot haciendo clic en el ícono ✨.
5. Intenta el prompt nuevamente. Si persiste, cierra Excel completamente, espera 30 segundos y reabre el archivo desde OneDrive.

---

### Problema 2: La tabla de sensibilidad muestra el mismo valor en todas las celdas o errores

**Síntomas:** Después de ejecutar **Datos → Análisis de hipótesis → Tabla de datos**, todas las celdas del rango muestran el mismo número, muestran ceros, o aparece el error `#¡VALOR!` en toda la tabla.

**Causa:** Este problema ocurre por una de estas razones:
- La **celda de esquina** (intersección de fila de encabezado y columna de encabezado) no contiene una fórmula que referencia las celdas de entrada correctas.
- Las **celdas de entrada de fila y columna** seleccionadas en el diálogo de Tabla de datos no corresponden a las variables que la fórmula de la celda de esquina utiliza.
- El rango seleccionado antes de ejecutar Tabla de datos no incluye la celda de esquina, o incluye celdas fuera del rango esperado.

**Solución:**
1. **Elimina la tabla de sensibilidad actual:** selecciona todas las celdas de resultados (no los encabezados de fila y columna), presiona **Supr**.
2. Verifica la **celda de esquina** (ej. D22): debe contener una fórmula como `=F14` (referencia directa a la celda de Utilidad Bruta Mensual del escenario Base). No debe contener un valor fijo.
3. Verifica que la fórmula de utilidad bruta en F14 depende de las celdas B4 (costo unitario) y B7 (volumen mensual). Traza las precedentes: selecciona F14 → **Fórmulas → Rastrear precedentes** y confirma que las flechas llegan a B4 y B7 (directa o indirectamente).
4. Selecciona **exactamente** el rango completo: desde la celda de esquina (D22) hasta la última celda de resultados (ej. I31). No incluyas filas o columnas adicionales.
5. Ve a **Datos → Análisis de hipótesis → Tabla de datos**.
6. En **Celda de entrada de fila**: haz clic en la celda **B7** (volumen mensual — corresponde a la variable del eje horizontal).
7. En **Celda de entrada de columna**: haz clic en la celda **B4** (costo unitario — corresponde a la variable del eje vertical).
8. Haz clic en **Aceptar**. Los resultados deben variar entre celdas, con valores más altos en la esquina superior derecha (bajo costo + alto volumen).

---

## Limpieza

1. **No elimines** el archivo `M2_Estrategia_Comercial_Precios.xlsx`. Este archivo es insumo obligatorio para los Módulos 3 y 4 del curso.

2. Puedes eliminar el archivo auxiliar `Notas_Insights_M1.txt` de la carpeta `M2_Estrategia_Comercial` si lo deseas, ya que su contenido fue incorporado en los prompts y no se referencia en módulos posteriores.

3. Verifica la estructura final de carpetas en OneDrive:

```
OneDrive/
└── Documentos/
    └── CopilotComunicacionEstrategia/
        ├── M1_Informe_Ejecutivo/
        │   └── M1_Informe_Ejecutivo_Posicionamiento.docx  ← conservar
        ├── M2_Estrategia_Comercial/
        │   └── M2_Estrategia_Comercial_Precios.xlsx       ← entregable de este lab
        ├── M3_Kit_Comunicacion/                            ← vacía (se usará en Módulo 3)
        └── M4_Brief_Presentacion/                          ← vacía (se usará en Módulo 4)
```

4. Cierra el panel lateral de Copilot en Excel y Word si no continuarás trabajando inmediatamente.

5. Si trabajaste en una computadora compartida, cierra sesión de tu cuenta de Microsoft 365 en todas las aplicaciones.

---

## Resumen

En este laboratorio construiste una estrategia comercial completa para Marca Nexo en un solo libro de Excel con cinco hojas interconectadas:

| Hoja | Contenido creado | Técnica de Copilot utilizada |
|---|---|---|
| `Matriz_Canales` | Estrategia diferenciada para 4 canales con roles, KPIs y tácticas | Generación de contenido estratégico en tablas |
| `Portafolio_Productos` | 8 SKUs con clasificación BCG, roles y canal preferente | Creación de datos estructurados con marcos analíticos |
| `Simulacion_Precios` | 3 escenarios de precios con fórmulas dinámicas + sensibilidad | Generación de fórmulas mediante lenguaje natural |
| `Plan_Piloto` | Cronograma de 90 días + métricas Go/No-Go | Diseño de planes operativos con criterios de decisión |
| `Resumen_Ejecutivo` | Narrativa ejecutiva integradora | Síntesis y análisis de datos tabulares |

**Conceptos clave reforzados:**
- La referencia cruzada entre módulos (M1 → M2) demuestra cómo Copilot genera mayor valor cuando recibe contexto acumulado.
- Las fórmulas dinámicas vinculadas a una tabla de Variables permiten simulación instantánea de escenarios sin reprogramar el modelo.
- El formato de Tabla de Excel es requisito técnico indispensable para que Copilot interactúe con datos en hojas de cálculo.
- Un plan piloto con criterios Go/No-Go cuantificados transforma una hipótesis de precios en una decisión ejecutiva estructurada.

### Próximos pasos

- **Módulo 3:** Utilizarás el archivo `M2_Estrategia_Comercial_Precios.xlsx` como insumo para construir kits de comunicación diferenciados por audiencia (distribuidor, punto de venta, consumidor) en `M3_Kit_Comunicacion_Distribuidores.docx`.
- **Práctica recomendada:** Antes del Módulo 3, experimenta cambiando los valores de la tabla de Variables en la hoja `Simulacion_Precios` para observar cómo se comportan los escenarios con diferentes supuestos. Prueba con el costo unitario en 1.50 y el volumen en 35,000 para simular un escenario pesimista.

### Recursos adicionales

- [Copilot en Excel — Documentación oficial de Microsoft](https://support.microsoft.com/es-es/copilot-excel)
- [Crear y dar formato a tablas en Excel](https://support.microsoft.com/es-es/office/crear-y-dar-formato-a-tablas-e81aa349-b006-4f8a-9806-5af9df0ac664)
- [Análisis de hipótesis con tablas de datos en Excel](https://support.microsoft.com/es-es/office/calcular-varios-resultados-con-una-tabla-de-datos-e95e2487-6ca6-4e62-9a17-827ce582e3c2)
- [Matriz BCG — Harvard Business School Online](https://online.hbs.edu/blog/post/bcg-matrix)
- [Estrategia de precios y canales — McKinsey & Company](https://www.mckinsey.com/capabilities/growth-marketing-and-sales/our-insights)
