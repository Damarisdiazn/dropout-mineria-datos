# Predicción de deserción y éxito académico en educación superior

**Asignatura:** Minería de Datos (UEA-L-UFPTI-009) · Universidad Estatal Amazónica
**Práctica:** Guía de Práctica Experimental N.º 1 – Minería de datos aplicada sobre un caso de estudio
**Integrantes:** _Nombre Apellido_, _Nombre Apellido_, _Nombre Apellido_

## 1. Descripción del problema
El abandono y el fracaso académico en educación superior afectan a estudiantes, instituciones y sociedad. Este proyecto aplica técnicas de minería de datos para clasificar el resultado académico de cada estudiante (*Dropout*, *Enrolled*, *Graduate*) y para descubrir perfiles de riesgo, de modo que tutores y coordinadores puedan intervenir a tiempo.

### Objetivos específicos
1. Explorar y caracterizar el dataset (estadísticas descriptivas, visualizaciones, nulos, duplicados y atípicos).
2. Preprocesar los datos: limpieza, codificación, normalización y variables derivadas.
3. Implementar y comparar árbol de decisión, Random Forest y regresión logística.
4. Evaluar con accuracy, F1 macro y validación cruzada de 5 particiones, e interpretar resultados.
5. Segmentar estudiantes con K-means para identificar perfiles de riesgo.

## 2. Datos
Ver [`data/raw/DATA_SOURCE.md`](data/raw/DATA_SOURCE.md). 4424 registros, 35 atributos + variable objetivo.

## 3. Estructura del repositorio
```
├── data/raw/          datos originales (no se versionan los CSV)
├── data/processed/    datos limpios con variables derivadas
├── notebooks/         01_eda_preprocesamiento · 02_modelado · 03_evaluacion
├── src/               funciones reutilizables
├── reports/figures/   gráficos
├── reports/tables/    tablas (incluye la tabla comparativa de modelos)
└── docs/              artículo IEEE y documento final
```

## 4. Instalación y ejecución
```bash
git clone <URL-DEL-REPOSITORIO>
cd dropout-mineria-datos
python -m venv .venv
# Windows: .venv\Scripts\activate    |  Linux/Mac: source .venv/bin/activate
pip install -r requirements.txt
jupyter notebook   # o abrir los notebooks en VS Code
```
Ejecutar los notebooks en orden numérico. Semilla global: `random_state=42`.

## 5. Resultados
_Completar al terminar: tabla comparativa de modelos (accuracy, F1 macro, media ± desv. de CV 5-fold) y hallazgos principales._

| Modelo | Accuracy (test) | F1 macro (test) | F1 macro CV (5-fold) |
|---|---|---|---|
| Árbol de decisión | | | |
| Random Forest | | | |
| Regresión logística | | | |

## 6. Cómo citar
Realinho, V., Vieira Martins, M., Machado, J., & Baptista, L. (2021). *Predict students' dropout and academic success* [Dataset]. UCI Machine Learning Repository. https://archive.ics.uci.edu/dataset/697

## 7. Licencia
MIT (código). Los datos mantienen la licencia de su fuente original.
