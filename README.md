# Dashboard: ¿Invertir más en educación reduce el desempleo en Colombia?

## Laboratorio Final – Semana 3

---

## Instrucciones de instalación y ejecución

### 1. Requisitos previos
- Python 3.9 o superior instalado
- pip actualizado

### 2. Instalar dependencias

```bash
pip install -r requirements.txt
```

### 3. Ejecutar el dashboard

```bash
streamlit run dashboard_educacion_colombia.py
```

El dashboard abrirá automáticamente en tu navegador en: http://localhost:8501

---

## Estructura del proyecto

```
/
├── dashboard_educacion_colombia.py   ← App principal Streamlit
├── requirements.txt                  ← Dependencias
└── README.md                         ← Este archivo
```

---

##  ¿Qué incluye el dashboard?

### Narrativa visual (3 fases del taller 1):
1. **Reto 1 replicado** – Gráfico dual línea (educación % PIB vs desempleo %)
2. **Reto 2** – Comparación LATAM con barchart de correlaciones
3. **Reto 3** – Scatter plot con línea de tendencia y anotaciones

### Filtros interactivos:
-  **Rango de años** (2010–2023)
-  **Países LATAM** para comparar (Chile, México, Perú, Brasil, Argentina)
-  **Modo de visualización** (líneas / área sombreada)

### KPIs en tiempo real:
- Inversión en educación (% PIB) último año
- Tasa de desempleo último año
- Correlación educación–desempleo
- País LATAM más efectivo en la relación

---

## Fuentes de datos

| Fuente | Variables |
|--------|-----------|
| Banco Mundial | Inversión en educación (% del PIB), 6 países LATAM |
| DANE (GEIH) | Tasa de desempleo Colombia |
| OCDE | Benchmarks de referencia |

> **Nota:** Los datos están simulados de forma realista para reflejar las tendencias reales del período 2010–2023. Para producción, reemplazar con datos oficiales del API del Banco Mundial.

---

## Estructura del código

```python
# 1. Configuración de página y CSS corporativo
# 2. Generación de datos simulados (función cacheada)
# 3. Sidebar con filtros reactivos
# 4. Hero block con veredicto ejecutivo
# 5. KPIs dinámicos (se actualizan con filtros)
# 6. Sección 1: Gráfico dual educación vs desempleo
# 7. Sección 2: Comparación LATAM
# 8. Sección 3: Scatter con tendencia
# 9. Recomendaciones ejecutivas
# 10. Footer
```

