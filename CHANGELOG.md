# Changelog

Todos los cambios relevantes de este proyecto se documentan en este archivo.
Formato: `[Versión] - [Fecha] / Añadido / Cambiado / Eliminado`.

## [1.1] - 2026-08-09

Línea base aprobada por el Change Control Board (CCB) tras la inspección Fagan
del ERS v1.0 (18 defectos registrados en el Anexo B) y la tramitación de tres
RFC. Corresponde al tag `baseline-v1.1`.

### Añadido
- **RF-26 — Moderar automáticamente los mensajes entre usuarios** (RFC-01):
  nuevo requisito funcional que da soporte a RNF-15 (explicabilidad de la
  moderación), hoy sin RF que lo especificara (defecto D-14).
- **CU-14 — Aviso de mascota extraviada sin contacto directo** (RFC-03): nuevo
  caso de uso que canaliza el contacto por mensajería interna (RF-07) en
  lugar de publicar datos de contacto.
- Fila **TR-51** en la matriz de trazabilidad, enlazando RF-26 con CU-08 y
  RNF-15 (RFC-01).
- Suposición sobre disponibilidad de datos de entrenamiento (mensajes
  etiquetados en español) para el componente de moderación automática,
  en la Sección 2.6 (defecto D-12, ligado a RFC-01).
- RF-25 incorporado a la tabla legal RL-05 (minimización de datos, LOPDP
  Art. 10 lit. e) (RFC-03).

### Cambiado
- **RF-07** (mensajería interna): prioridad MoSCoW elevada de *Could* a
  *Must* (condición conjunta de RFC-01 y RFC-03), al convertirse en la única
  vía de contacto sustituta para RF-25 y en requisito padre de RF-26.
- **RF-25** (aviso de mascota extraviada): reformulado para no publicar datos
  de contacto directo; el contacto se canaliza vía RF-07 y la ubicación se
  publica con granularidad reducida (sector o parroquia) (RFC-03, defecto
  D-09, crítico).
- **RNF-09** y **RD-08** (notificaciones externas): reformulados para ser
  neutrales respecto del proveedor, retirando la mención nominal a WhatsApp
  Business API y elevando el canal de respaldo in-app de recomendación a
  obligación (RFC-02, defecto D-06).
- Fila **TR-38** de la matriz de trazabilidad corregida: eliminada la
  asignación duplicada de CU-04 a RF-25 (RFC-03).
- 11 defectos mayores y críticos del Anexo B corregidos directamente sobre el
  ERS (sin tramitación por CCB): D-03, D-05, D-07, D-08, D-11, D-15, D-16,
  D-17, D-18, y ajustes asociados a D-12.
- Historial de versiones y portada del ERS actualizados de v1.0 a v1.1.

### Eliminado
- **"Sugerencias inteligentes para completar perfiles"** y
  **"Recomendaciones básicas de cuidado"** retiradas del alcance del producto
  (Sección 1.2): ninguna contaba con evidencia de campo ni figuraba en la
  matriz de trazabilidad (RFC-01, defecto D-02).
- Compromiso nominal con WhatsApp Business API como proveedor único de
  notificaciones (RFC-02).
- Publicación pública de datos de contacto directo en el aviso de mascota
  extraviada (RF-25) (RFC-03).

---

## [1.0] - 2026-07-29

Entrega 3 (2A): ERS/SRS completo. 25 RF, 16 RNF y 9 RD; requisitos legales,
explicabilidad, historias de usuario, modelado UML completo, priorización
Kano/WSJF, trazabilidad extendida, MVP y componente empírico.
