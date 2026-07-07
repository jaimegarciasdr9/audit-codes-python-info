# Audit Codes Python

Repositorio de scripts Python de uso profesional en auditoría y análisis financiero.

> El código fuente es privado. Para solicitar acceso, abre un Issue usando el botón de abajo.

**[➜ Solicitar acceso al código](https://github.com/jaimegarciasdr9/audit-codes-python-info/issues/new?title=Solicitud+de+acceso&body=Hola%2C+me+gustar%C3%ADa+acceder+al+c%C3%B3digo+del+repositorio.%0A%0ANombre%3A+%0AMotivo%3A+)**

---

## Proyectos disponibles

### IFRS9 — Riesgo de Crédito

Réplica de modelos de riesgo de crédito para auditoría IFRS9 (LEVAs).

| Módulo | Descripción |
|---|---|
| `01_replica_PD_GT` | Réplica del modelo de Probabilidad de Default (PD) mediante regresión logística |
| `02_replica_LGD_GT` | Réplica del modelo de Severidad / Loss Given Default (LGD) |
| `03_calculo_reservas` | Cálculo de reservas IFRS9 a partir de los modelos PD y LGD |

**Stack:** Python · pandas · numpy · statsmodels

---

### NAV — Valores Liquidativos

Obtención automatizada de valores liquidativos (NAV) de fondos de inversión desde múltiples fuentes.

| Módulo | Descripción |
|---|---|
| `get_nav_cnmv` | Descarga de NAV desde el registro oficial de la CNMV |
| `nav_todos` | Agregación de NAV de todos los fondos (Yahoo Finance + CNMV) |
| `nav_yahoo` | Consulta de NAV por ISIN desde Yahoo Finance |
| `yahoo_finance` | Capa de conexión y utilidades con la API de Yahoo Finance |
| `valor_liquidativo` | Cálculo del valor liquidativo neto |

**Stack:** Python · yfinance · requests · pandas

---

### Utils — Utilidades

| Módulo | Descripción |
|---|---|
| `extraer_dnis` | Extrae y cuenta DNIs/NIEs de documentos PDF con texto seleccionable |

**Stack:** Python · pdfplumber · re

---

## Solicitar acceso

El repositorio con el código fuente es privado.  
Para solicitar acceso, abre un Issue y lo gestiono en menos de 24h.

**[➜ Abrir solicitud de acceso](https://github.com/jaimegarciasdr9/audit-codes-python-info/issues/new?title=Solicitud+de+acceso&body=Hola%2C+me+gustar%C3%ADa+acceder+al+c%C3%B3digo+del+repositorio.%0A%0ANombre%3A+%0AMotivo%3A+)**
