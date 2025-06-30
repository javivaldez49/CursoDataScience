# 🚔 ¿Dónde se roban más autos?  
### Un análisis de denuncias por robos y hurtos vehiculares en Argentina

📍 Proyecto de análisis de datos sobre denuncias de robos y recuperos de automotores en Argentina.  
🔗 [Accedé al proyecto en Google Colab](https://colab.research.google.com/drive/1vX67IsvwLIR-nLEGmhyHghslem65lZiM?usp=sharing)

---

## 📚 Contexto

Los datos analizados provienen de los Registros Seccionales de la Propiedad del Automotor y Créditos Prendarios.  
Este conjunto de datos refleja la cantidad de trámites relacionados con robos, hurtos y recuperos de vehículos en diferentes provincias de Argentina.  
La información es útil para detectar zonas con mayor concentración de denuncias, así como patrones vinculados a marcas, modelos y características del titular.

---

## ✅ Resultados principales

- 📌 **Provincias con más denuncias**: Buenos Aires, CABA y Santa Fe lideran en cantidad de casos.  
- 🚗 **Marcas más robadas**: Volkswagen, Chevrolet y Fiat encabezan el ranking.  
- 📍 **Zonas de denuncia frecuentes**: La Matanza, Lomas de Zamora y Esteban Echeverría son los registros más comunes.  
- 🎯 **Precisión del modelo de clasificación**: ~83% de accuracy utilizando un modelo supervisado.

---

## 🛠️ Tecnologías y herramientas utilizadas

- 💻 **Google Colab** – Entorno de trabajo colaborativo basado en la nube  
- 🐍 **Python** – Lenguaje principal del proyecto  
- 🧮 **Pandas** – Limpieza y manipulación de datos  
- 📊 **Matplotlib & Seaborn** – Visualización de datos  
- 🤖 **Scikit-learn** – Implementación de machine learning:
  - `train_test_split`, `LabelEncoder`, `SelectKBest`, `chi2`
  - `RandomForestClassifier` + métricas (`accuracy_score`, `classification_report`, `confusion_matrix`)

---

## 🔎 Metodología

1. 📂 Carga del dataset en formato `.xlsm` desde Google Drive  
2. 🧹 Limpieza de datos: detección de valores nulos, codificación de variables categóricas y selección de variables relevantes  
3. 📈 Análisis exploratorio: visualización de frecuencia de denuncias por provincia, marca y seccional  
4. 🧠 Modelado: entrenamiento de un modelo de clasificación para predecir el lugar de denuncia según variables del vehículo y del titular  
5. 📊 Evaluación del modelo: se calcularon métricas de desempeño y se analizaron los resultados

---

## 🔗 Fuente

Los datos provienen de la plataforma de datos abiertos del Gobierno de la Provincia de Buenos Aires:  
📎 [https://datos.gob.ar/dataset/justicia-robos-recuperos-autos](https://datos.gob.ar/dataset/justicia-robos-recuperos-autos)

---

## 💡 Conclusiones y aprendizajes

- Existen fuertes concentraciones geográficas de robos, especialmente en zonas del conurbano bonaerense  
- Las marcas más populares son también las más robadas, posiblemente por su disponibilidad en el mercado  
- El modelo predictivo tuvo buen rendimiento, lo que sugiere que variables como año, marca del vehículo y género del titular están asociadas al lugar de denuncia  
- Aprendí a integrar visualización de datos, limpieza, modelado y evaluación en un flujo de trabajo de ciencia de datos completo 🚀

