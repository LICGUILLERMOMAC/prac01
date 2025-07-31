## Práctica 4: Análisis de Riesgo de enfermedad por hábitos diarios

---

### 👥 Integrantes de Equipo:

- Edgar Ivan Lozada Sanchez
- Luis Antonio Guerrero Ibarra
- Emma Edith Martínez Méndez
- Elias Cuahutencos Rojas
- Guillermo Armando Lopez Ayala

---

### 📌 Descripción del Proyecto

Este proyecto tiene como objetivo desarrollar e implementar una biblioteca modular en Python para realizar el procesamiento y análisis de datos sobre el dataset **"Disease Risk from Daily Habits"** mediante técnicas de análisis exploratorio, selección y transformación de variables, con el fin de mejorar la eficiencia y precisión de modelos predictivos.

---

### 📝 Funcionalidades Principales

La biblioteca está organizada en módulos independientes pero integrables, que permiten realizar principalmente las siguientes tareas:
    
**Funciones** 
        
1. *Information Value (IV) y Weight of Evidence (WoE):* Este módulo calcula métricas IV y WoE, útiles para evaluar la relación entre variables independientes y la variable objetivo.

2. *Análisis de Componentes Principales (PCA):* Emplea PCA, permitiendo reducir el número de variables manteniendo la mayor parte de la varianza explicada. Este componente es parametrizable para adaptarse a distintos umbrales de varianza acumulada.

3. *SelectBest:* Se integra un módulo que implementa métodos como SelectKBest para identificar las variables con mayor relevancia predictiva.

4. *Análisis de multicolinealidad:* Emplea la técnica de VarClusHi para realizar el agrupamiento jerárquico de varables, basada en la correlación entre ellas para identificar cluster o grupos de variables altamente correlacionadas.

**Gráficas**  

Generación de visualizaciones para explorar la relación entre las variables mediante los siguientes gráficos:

* Boxplots
* Histogramas
* Scatter Plots
* PCA 3D
* PCA 2D

**Preprocessing**

Se integra de los siguientes procesos:
* Estadisticas Descriptivas
* Identificación de valores faltantes, nulos y tipo de datos
* Tratamiento de valores faltantes y atipicos mediante IQR
* Codificación

---

### 🛠️ Herramientas

    1. Visual Studio Code
    2. Python  3.11.9

---

### 🧩 Estructura del Proyecto

La instalación de la siguiente libreria, se deberá trabajar dentro de la carpeta  ```h_life_class```, es recomendado trabajar en un entorno vitual con los siguientes códigos en esa ubicación:

    h_life_class/
    ├── funciones/
    │   ├── _init_.py
    │   ├── CalculodeIVyWoE.py
    │   ├── PCA.py
    │   ├── SelectKbest.py
    │   └── VarClushHi.py
    │
    ├── plots/
    │   ├── _init_.py
    │   ├── boxplots.py
    │   ├── histograms.py
    │   └── scatter_plots.py
    │
    ├── setup.py
    ├── preprocessing.py
    ├── requirements.txt
    ├── P4.ipynb
    └── README.md 
---

### 🎯 Contenido de Archivos Integrados

📄 ```requirements.txt```

Librerias:

    - pandas==2.3.1
    - numpy==2.3.2
    - scikit-learn==1.7.1
    - scipy==1.16.1
    - plotly==5.18.0
    - cufflinks==0.17.3
    - seaborn==0.13.2
    - matplotlib==3.10.3
    - factor-analyzer==0.3.1
    - colorlover==0.3.0
    - varclushi==0.1.0
    - ipywidgets==8.1.7 
    - nbformat>=5.10.4

> En caso de uso de Jupyter se deberá instalar Jupyter Notebook:

    pip install -r requirements.txt

---

### ✅ Ejemplo de uso básico

    from h_life_class.funciones import varclushi_representantes

    RVCHXmm = varclushi_representantes(Xmm)
    print("\nVariables candidatas para quedarse como representativas del clúster:")

---
### 📦 Descripción del Dataset

* **Archivo**: ```health_lifestyle_dataset.csv```
* **Dimensiones**: 100,000 filas y 41 columnas (incluyendo la variable target).

## Las gráficas son interactivas para optimizar la visualización y el análisis de los datos.

![GRAFICA_A ](https://github.com/LICGUILLERMOMAC/prac01/blob/a36a72f68e747f706f183295cab4a4cc3df35151/WhatsApp%20Image%202025-07-30%20at%2010.35.31%20PM.jpeg)

![GRAFICA_B ](https://github.com/LICGUILLERMOMAC/prac01/blob/a36a72f68e747f706f183295cab4a4cc3df35151/WhatsApp%20Image%202025-07-30%20at%2010.35.32%20PM%20(1).jpeg)

![GRAFICA_c ](https://github.com/LICGUILLERMOMAC/prac01/blob/a36a72f68e747f706f183295cab4a4cc3df35151/WhatsApp%20Image%202025-07-30%20at%2010.35.32%20PM.jpeg)




