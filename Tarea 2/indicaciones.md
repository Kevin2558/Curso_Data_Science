# Tarea 2, parte 1 — Reducción de Dimensionalidad (solo pre-procesamiento)

> **Objetivo:** practicar distintas técnicas de reducción de variables  

---

## Instrucciones generales

1. Descarga el dataset indicado desde Kaggle.  
2. Carga los datos en un notebook (`pandas`) e inspecciona su forma *(filas × columnas)*.  
3. Estandariza las variables numéricas cuando corresponda (`StandardScaler`).  
4. Aplica la técnica de reducción solicitada.  
5. Reporta en tu notebook:  
   - **Número de componentes** retenidos.  
   - **Porcentaje de varianza explicada** (o criterio equivalente).  
   - Una **visualización 2-D** o 3-D (scatter) coloreada con la etiqueta disponible, si existe.  
   - Una breve conclusión (2-3 frases) sobre si la proyección revela estructura o correlaciones.

---

## Lista de ejercicios

| # | Dataset (Kaggle slug) | Tipo / Dimensión | Técnica de reducción solicitada |
|---|-----------------------|------------------|---------------------------------|
| 1 | `zalando-research/fashionmnist` | 70 000 × 784 (imágenes) | **PCA** → conservar 95 % de la varianza |
| 2 | `mchrishtw/human-activity-recognition-with-smartphones` | 10 299 × 561 (sensores) | **PCA** (scree plot) + **ICA** (10 componentes); compara varianza vs. independencia |
| 3 | `wine-quality` | 6 497 × 11 (químico) | **LDA** (proyección supervisada) → 2 componentes y scatter tintos vs. blancos |
| 4 | `credit-card-fraud` | 284 807 × 30 (numérico) | **t-SNE** y **UMAP** a 2 D; colorea fraude / no fraude |
| 5 | `uci-ml/energy-efficiency` | 768 × 8 (regresión) | **PCA** a 2 D; muestra por qué a veces la reducción **no** es necesaria (varianza explicada ≥ 90 %?) |

---

### Entrega

- Notebook (.ipynb) bien comentado.  
- Incluye gráficos y celdas con los valores de varianza explicada / independencia.  
- Una sección final “Conclusiones” (máx. ½ página) donde resumas qué técnica te pareció más informativa para cada dataset.
