# ISR401-PFC-ERS-EquipoD

## MundiPets — Plataforma para el cruce y la adopción responsable de mascotas

Repositorio correspondiente a la **Práctica Experimental PE4 – Unidad IV** de la asignatura **Ingeniería de Requerimientos (ISR-401)** de la Universidad Técnica Estatal de Quevedo.

El trabajo aplica técnicas de **validación de requisitos, inspección Fagan, gestión del cambio mediante un Change Control Board (CCB), trazabilidad en una herramienta CASE y control de versiones mediante Git** sobre el ERS real del Proyecto Fin de Curso **MundiPets**.

---

## 📌 Información del proyecto

| Elemento | Información |
|---|---|
| **Proyecto PFC** | MundiPets |
| **Descripción** | Plataforma para el cruce y la adopción responsable de mascotas |
| **Asignatura** | Ingeniería de Requerimientos (ISR-401) |
| **Unidad** | Unidad IV — Validación, Gestión de Requisitos y Herramientas CASE |
| **Equipo** | Equipo D |
| **ERS inicial** | Versión 1.0 |
| **ERS actualizado** | Versión 1.1 |
| **Línea base** | `baseline-v1.1` |
| **Herramienta CASE** | Jira |
| **Control de versiones** | Git / GitHub |
| **Informe** | LaTeX + BibLaTeX + Biber |

Repositorio oficial: **ISR401-PFC-ERS-EquipoD**

---

## 👥 Integrantes

| Integrante | Rol en la práctica |
|---|---|
| **Gary Alejandro Morales Sánchez** | Moderador |
| **Gary Alberto Sánchez Cornejo** | Lector + Inspector 1 |
| **Wilson Lizandro Cedeño Coronado** | Inspector 2 |

Los roles fueron definidos para la inspección formal del ERS de acuerdo con el método Fagan.

---

## 🎯 Objetivos de la práctica

La práctica tiene como objetivos principales:

- Ejecutar una inspección formal tipo **Fagan** sobre el ERS de MundiPets.
- Identificar, clasificar y corregir defectos de requisitos.
- Calcular e interpretar métricas de inspección.
- Gestionar tres solicitudes formales de cambio (**RFC**).
- Realizar una simulación de **Change Control Board (CCB)**.
- Implementar trazabilidad bidireccional de requisitos mediante **Jira**.
- Establecer una línea base del ERS mediante **Git**.
- Comparar herramientas CASE para Ingeniería de Requisitos.
- Contrastar la Ingeniería de Requisitos tradicional frente a la Ingeniería de Requisitos ágil.

La rúbrica establece que el repositorio debe contener el ERS versionado, la línea base y los anexos correspondientes a la práctica.

---

## 🔎 Inspección Fagan

La inspección formal se realizó sobre la **ERS versión 1.0**, con una extensión de **147 páginas**.

Durante la inspección:

- Se utilizaron roles diferenciados.
- Se realizó preparación individual de los inspectores.
- Se efectuó una reunión de consolidación.
- Se identificaron **18 defectos únicos**.
- Los defectos fueron clasificados por tipo y severidad.
- Se analizaron las propiedades de:
  - Ambigüedad
  - Completitud
  - Consistencia
  - Verificabilidad
  - Trazabilidad
  - Factibilidad

También se calcularon cinco métricas de inspección:

1. Densidad de defectos.
2. Distribución de defectos por tipo.
3. Distribución de defectos por severidad.
4. Tasa de detección por inspector.
5. Esfuerzo total en horas-persona.

La rúbrica exige un mínimo de **15 defectos únicos**, al menos **3 críticos o mayores**, además de las cinco métricas calculadas, graficadas e interpretadas.

---

## 🔄 Gestión del cambio y CCB

A partir de los defectos encontrados se gestionaron tres solicitudes formales de cambio:

| RFC | Tipo | Descripción |
|---|---|---|
| **RFC-01** | Alcance | Incorporación de RF-26 y retiro de funciones sin evidencia suficiente |
| **RFC-02** | Calidad | Modificación de requisitos relacionados con proveedor y restricciones |
| **RFC-03** | Normativa / restricción | Resolución del conflicto entre RF-25 y RNF-16 |

Las tres RFC fueron analizadas mediante la matriz de trazabilidad y posteriormente evaluadas por el **Change Control Board (CCB)**.

Como resultado de la gestión del cambio se obtuvo la **versión 1.1 del ERS**.

La rúbrica exige que cada RFC incluya el requisito afectado, justificación, requisitos impactados, artefactos afectados, esfuerzo, riesgo y recomendación técnica, además de una decisión motivada del CCB.

---

## 🔗 Trazabilidad

La trazabilidad de requisitos se implementó utilizando **Jira**.

El tablero organiza los requisitos mediante áreas funcionales y utiliza campos personalizados, incluyendo:

- Prioridad **MoSCoW**.
- Fuente del requisito.
- Estado de verificación.

La trazabilidad se establece en ambas direcciones:

```text
Stakeholder
     ↓
Requisito funcional (RF)
     ↓
Caso de uso (CU)
     ↓
Clase / Módulo
     ↓
Prueba
```

La matriz de trazabilidad desarrollada contiene **26 filas**, correspondientes a los requisitos funcionales del sistema.

La estructura exigida por la rúbrica contempla como mínimo **4 Epics, 15 Stories, sub-tareas para criterios de aceptación, dos campos personalizados y trazabilidad bidireccional**.

---

## 🏷️ Línea base y control de versiones

La versión final aprobada del ERS corresponde a:

```text
ERS v1.1
```

La línea base se identifica mediante el tag:

```text
baseline-v1.1
```

La línea base representa la versión del ERS resultante después de la evaluación y aprobación de los cambios realizados mediante el CCB.

También se mantiene un `CHANGELOG.md` para registrar las modificaciones realizadas y asociarlas con las RFC correspondientes.

La rúbrica exige que la versión declarada en el ERS, el historial, el `CHANGELOG.md` y el tag de Git sean coherentes.

---

## 📁 Estructura del repositorio

La organización del repositorio sigue la estructura propuesta en la guía de la práctica:

```text
ISR401-PFC-ERS-EquipoD/
│
├── README.md
├── CHANGELOG.md
│
├── 01_ERS/
│   ├── ERS_v1.0.pdf
│   ├── ERS_v1.1.pdf
│   └── fuentes/
│       ├── *.tex
│       └── referencias.bib
│
├── 02_Inspeccion/
│   ├── AnexoA_checklists/
│   ├── AnexoB_registro_defectos.xlsx
│   └── metricas.xlsx
│
├── 03_CCB/
│   ├── RFC-01.pdf
│   ├── RFC-02.pdf
│   ├── RFC-03.pdf
│   └── Acta_CCB.pdf
│
├── 04_Trazabilidad/
│   ├── matriz_trazabilidad.xlsx
│   ├── backlog_export.csv
│   └── capturas/
│
├── 05_Informe/
│   ├── PE4_U4_MORALES_SANCHEZ_CORNEJO_CEDENO.tex
│   ├── referencias.bib
│   ├── PE4_U4_MORALES_SANCHEZ_CORNEJO_CEDENO.pdf
│   └── figuras/
│
└── 06_Evidencias/
    ├── capturas_git/
    ├── fotos_sesion/
    └── declaracion_IA.pdf
```

Esta organización responde a la estructura de repositorio indicada por la guía, que contempla ERS, inspección, CCB, trazabilidad, informe y evidencias.

---

# 🛠️ Compilación del informe LaTeX

## Requisitos

Para generar el informe se necesita:

- **LaTeX** mediante MiKTeX o TeX Live.
- **Biber**.
- Clase `IEEEtran`.
- Paquetes utilizados por el documento.
- Archivos de figuras incluidos en la carpeta `figuras/`.
- Archivo bibliográfico `referencias.bib`.

La guía de la práctica contempla MiKTeX o TeX Live como distribuciones para compilar el informe.

## Archivo principal

El archivo principal del informe es:

```text
PE4_U4_MORALES_SANCHEZ_CORNEJO_CEDENO.tex
```

El documento utiliza:

```text
IEEEtran
biblatex
Biber
```

y la bibliografía se encuentra en:

```text
referencias.bib
```

## Compilación mediante terminal

Ubicarse en la carpeta donde se encuentra el archivo `.tex` y ejecutar:

```bash
pdflatex PE4_U4_MORALES_SANCHEZ_CORNEJO_CEDENO.tex
biber PE4_U4_MORALES_SANCHEZ_CORNEJO_CEDENO
pdflatex PE4_U4_MORALES_SANCHEZ_CORNEJO_CEDENO.tex
pdflatex PE4_U4_MORALES_SANCHEZ_CORNEJO_CEDENO.tex
```

El orden de ejecución es importante porque:

1. `pdflatex` genera los archivos auxiliares.
2. `biber` procesa las referencias bibliográficas.
3. `pdflatex` incorpora las referencias y citas.
4. La última compilación actualiza las referencias cruzadas, tablas e índice.

### Compilación con MiKTeX

En Windows también puede utilizarse:

```bash
pdflatex PE4_U4_MORALES_SANCHEZ_CORNEJO_CEDENO.tex
biber PE4_U4_MORALES_SANCHEZ_CORNEJO_CEDENO
pdflatex PE4_U4_MORALES_SANCHEZ_CORNEJO_CEDENO.tex
pdflatex PE4_U4_MORALES_SANCHEZ_CORNEJO_CEDENO.tex
```

Se recomienda tener habilitada la instalación automática de paquetes faltantes en MiKTeX.

---

## 📚 Dependencias LaTeX principales

El documento utiliza, entre otros, los siguientes paquetes:

```text
IEEEtran
fontenc
inputenc
babel
csquotes
booktabs
tabularx
array
multirow
longtable
graphicx
float
xcolor
geometry
fancyhdr
parskip
enumitem
amssymb
amsmath
titlesec
caption
listings
biblatex
hyperref
```

Las imágenes utilizadas por el informe se encuentran en la carpeta:

```text
figuras/
```

---

## 📊 Artefactos principales

El repositorio contiene los artefactos generados durante la práctica:

### ERS

- ERS versión 1.0.
- ERS versión 1.1.
- Fuentes LaTeX asociadas.

### Inspección Fagan

- Listas de verificación.
- Registro de defectos.
- Métricas de inspección.
- Evidencias de la sesión.

### Gestión del cambio

- RFC-01.
- RFC-02.
- RFC-03.
- Acta del CCB.
- ERS actualizado después de los cambios.

### Trazabilidad

- Matriz de trazabilidad.
- Exportación CSV del backlog.
- Evidencias del tablero Jira.
- Evidencias de los enlaces de trazabilidad.

### Línea base

- Historial de commits.
- Tag `baseline-v1.1`.
- `CHANGELOG.md`.
- Evidencias de GitHub.

### Informe

- Archivo `.tex`.
- Archivo `.bib`.
- PDF generado.
- Figuras utilizadas por el documento.

---

## 🤖 Uso de inteligencia artificial

Durante la elaboración de la práctica se utilizaron herramientas de inteligencia artificial como apoyo en determinadas tareas de redacción y estructuración.

El uso de IA fue declarado en el **Anexo F** del informe, indicando:

- Herramienta y versión.
- Tarea asistida.
- Fragmentos afectados.
- Verificación crítica realizada por el equipo.

Los datos técnicos, métricas, defectos, RFC, decisiones del CCB y elementos de trazabilidad fueron contrastados por el equipo con los artefactos correspondientes antes de incorporarlos al informe.

La guía establece que el uso de asistentes de IA debe declararse y que el contenido asistido debe ser sometido a verificación crítica.

---

## ✅ Criterios de reproducibilidad

Para comprobar que el informe puede reproducirse desde el repositorio:

1. Clonar el repositorio.
2. Verificar que el archivo `.tex`, `referencias.bib` y las figuras estén disponibles.
3. Instalar una distribución LaTeX compatible.
4. Verificar que Biber esté instalado.
5. Ejecutar los comandos de compilación indicados anteriormente.
6. Comprobar que se genera correctamente el PDF.

La rúbrica establece la reproducibilidad del PDF desde el código LaTeX como criterio de piso obligatorio.

---

## 📌 Línea base

La versión aprobada del proyecto se encuentra identificada mediante:

```text
baseline-v1.1
```

Para consultar la línea base:

```bash
git tag -n
```

Para consultar el historial:

```bash
git log --oneline --graph --decorate
```

La guía solicita un tag anotado y publicado, además del historial de Git como evidencia de la línea base.

---

## 📖 Referentes utilizados

El informe se fundamenta principalmente en:

- ISO/IEC/IEEE 29148:2018.
- ISO/IEC/IEEE 15288:2023.
- ISO/IEC/IEEE 12207:2017.
- ISO/IEC 25010:2023.
- Pohl, *Requirements Engineering*, 2.ª edición.
- SWEBOK Guide v4.0.
- PMBOK Guide, 7.ª edición.
- IREB CPRE FL v3.1.
- Fagan (1976).
- Cohn (2004).
- Smart (2014).

La guía establece estas fuentes como referentes para el fundamento teórico de la práctica.

---

## 📄 Informe

El informe corresponde a la **Práctica Experimental PE4 — Unidad IV: Validación, Gestión de Requisitos y Herramientas CASE**.

El documento integra:

- Fundamento teórico.
- Inspección Fagan.
- Correcciones aplicadas.
- Gestión del cambio y CCB.
- Trazabilidad en Jira.
- Línea base con Git.
- Comparativa de herramientas CASE.
- Comparación entre IR tradicional e IR ágil.
- Conclusiones críticas.
- Distribución del trabajo.
- Referencias.
- Anexos A–F.

---

## 🎓 Universidad Técnica Estatal de Quevedo

**Facultad de Ciencias de la Computación**  
**Carrera de Ingeniería en Software**  
**Asignatura:** Ingeniería de Requerimientos (ISR-401)  
**Unidad IV — Validación, Gestión de Requisitos y Herramientas CASE**  
**Periodo:** 2026–2027 PPA