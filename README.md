# IA-UPC-Grupo-Alvarado-Avalos-Espiritu-y-Risco
Integrantes: Cinthya Vanessa Alvarado Ruiz, Carlos Ernesto Gabriel Avalos Casachagua, Renzo Edgar Espiritu Garcia y Ana Risco Anton

Resistencia a la Compresión del Concreto
Tipo de Datos: Multivariado

## 1. Definición del Problema Estructural

El concreto es el material predominante en la ingeniería civil; sin embargo, la predicción de su resistencia a la compresión (f'c) representa un desafío complejo en Concretos de Alto Desempeño (HPC). Los métodos de diseño tradicionales empíricos resultan insuficientes al modelar la interacción altamente no lineal entre adiciones minerales, aditivos químicos y la edad de curado. 

El objetivo de este proyecto es desarrollar un modelo de Machine Learning capaz de predecir la resistencia a la compresión del concreto basándose en sus proporciones de mezcla, reduciendo la dependencia de ensayos destructivos a los 28 días y optimizando el uso de materiales para garantizar la seguridad estructural.

## 2. Descripción de los Datos (Dataset)

Se utiliza el **Concrete Compressive Strength Dataset**, extraído del UCI Machine Learning Repository. El dataset contiene resultados de ensayos de laboratorio controlados sin sesgos empíricos.

**Fuente de los Datos Originales:**

* **Propietario y Donante:**
Prof. I-Cheng Yeh
* **Institución:** Departamento de Gestión de la Información
Universidad Chung-Hua,
Hsin Chu, Taiwán 30067, R.O.C.
Correo electrónico: icyeh@chu.edu.tw
Teléfono: 886-3-5186511

* **Fecha de donación:** 3 de agosto de 2007

* **Publicación de referencia:** I-Cheng Yeh, "Modeling of strength of high performance concrete using artificial neural networks," Cement and Concrete Research, Vol. 28, No. 12, pp. 1797-1808 (1998).

**Características de la Base de Datos:**

La resistencia real a la compresión del concreto (MPa) para una mezcla determinada bajo una edad específica (días) se determinó en laboratorio. Los datos se encuentran en su formato original (no escalados).

* **Observaciones:** 1030 instancias.
* **Valores nulos:** Ninguno.
* **Variables:** 8 variables predictoras de entrada y 1 variable objetivo de salida.

A continuación se detalla el nombre de la variable, el tipo de variable, la unidad de medida y una breve descripción. La resistencia a la compresión del concreto representa el problema de regresión. El orden de este listado corresponde al orden numérico a lo largo de las filas de la base de datos.

| Variable | Tipo de Dato | Unidad | Rol |
| :--- | :--- | :--- | :--- |
| Cemento | Cuantitativo | kg/m³ | Entrada |
| Escoria de Alto Horno | Cuantitativo | kg/m³ | Entrada |
| Ceniza Volante | Cuantitativo | kg/m³ | Entrada |
| Agua | Cuantitativo | kg/m³ | Entrada |
| Superplastificante | Cuantitativo | kg/m³ | Entrada |
| Agregado Grueso | Cuantitativo | kg/m³ | Entrada |
| Agregado Fino | Cuantitativo | kg/m³ | Entrada |
| Edad | Cuantitativo | Días (1 - 365) | Entrada |
| **Resistencia a la Compresión** | **Cuantitativo** | **MPa** | **Salida (Target)** |

## 3. Marco Veridical Data Science (PCS)

Este proyecto se rige bajo los principios de *Veridical Data Science* (Yu & Barter, 2024):
* **Predictibilidad:** Validación de la captura de la física de hidratación mediante el rendimiento en datos no observados.
* **Computabilidad:** Flujo de trabajo transparente, escalable y reproducible programado íntegramente en Python.
* **Estabilidad:** Análisis de robustez para asegurar que las inferencias estructurales no se vean alteradas por perturbaciones aleatorias en los datos.

## 4. Estructura del Repositorio
El trabajo está dividido en entregas escalonadas (T1, T2, T3):

```text
├── data/               # Base de datos cruda y procesada (.csv, .xls)
├── docs/               # Informes, rúbricas y presentaciones (.pdf, .docx)
├── src/                # Scripts de Python y Jupyter Notebooks (.py, .ipynb)
└── README.md           # Descripción general del proyecto
```

## Agradecimientos, Información de Derechos de Autor y Disponibilidad
  
NOTA: La reutilización de esta base de datos es ilimitada, conservando el aviso de derechos de autor a favor del Prof. I-Cheng Yeh y del siguiente artículo publicado:  I-Cheng Yeh, "Modeling of strength of high performance concrete using artificial neural networks," Cement and Concrete Research, Vol. 28, No. 12, pp. 1797-1808 (1998).

