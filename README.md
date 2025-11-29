# ⚽ Inazuma Eleven — Equipo Definitivo 4-3-3 

Este proyecto analiza las estadísticas de los jugadores del videojuego Inazuma Eleven para construir el **mejor equipo posible utilizando la formación **4-3-3**.  
El objetivo es seleccionar a los 11 jugadores con mejor rendimiento global según sus estadísticas.

---

## 🚀 Objetivos del proyecto

- Cargar y explorar el dataset original de jugadores.
- Calcular una métrica global llamada `overall` basada en la media de sus estadísticas.
- Filtrar y seleccionar jugadores por posición:
  - 1 Portero (GK)
  - 4 Defensas (DF)
  - 3 Centrocampistas (MF)
  - 3 Delanteros (FW)
- Formar el Equipo Definitivo.

## 🛠 Tecnologías utilizadas

- **Python 3**
- **Pandas**
- **NumPy**
- **Jupyter Notebook**


## 📁 Estructura del proyecto

```
inazuma_ultimate_team/
│
├── data/                → dataset
├── notebooks/           → análisis principal
└── README.md            → documentación del proyecto

## 📊 Metodología

1️⃣ Preprocesamiento
- Carga del dataset.
- Revisión de duplicados y nulos.
- Identificación de las columnas de estadísticas numéricas:
  `Kick`, `Body`, `Control`, `Guard`, `Speed`, `Stamina`, `Guts`, `FP`, `TP`.

2️⃣ Creación de la métrica `overall`
Para cada jugador se calcula la media de sus estadísticas relevantes:

```
overall = mean([Kick, Body, Control, Guard, Speed, Stamina, Guts, FP, TP])
```

3️⃣ Selección de jugadores por posición

Se creó una función llamada:

```
mejores_por_posicion(df, posicion, n)
```

que devuelve los n mejores jugadores según `overall`.

Se seleccionaron:
- **1 GK**
- **4 DF**
- **3 MF**
- **3 FW**


## 💡 Conclusiones

- El equipo final representa a los jugadores más completos según la media de sus estadísticas.
- El método basado en la media es adecuado porque las estadísticas del juego ya están alineadas con cada posición.
- La formación 4-3-3 seleccionada combina equilibrio defensivo y ofensivo.

---

## 🔮 Mejoras futuras

- Aplicar ponderación específica para cada posición.
- Normalizar estadísticas para mayor precisión.
- Comparar diferentes modelos de selección de jugadores.
- Crear un dashboard interactivo en Power BI o Streamlit.

---

## 👤 Autor

Proyecto realizado por **Pablo Merenciano Moñino** como parte de su portfolio de análisis de datos.
