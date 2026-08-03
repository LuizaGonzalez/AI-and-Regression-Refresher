# Stellar Luminosity — Regresión Lineal y Polinómica

## Propósito
 
Este proyecto implementa, desde cero (sin librerías de machine learning), un modelo de regresión lineal y uno polinómico para estudiar la relación entre la masa y la luminosidad de una estrella. El objetivo es entender cómo aprende un modelo de regresión trabajando directamente con la predicción, el error, el gradiente, la optimización y las limitaciones del modelo.

## Librerías requeridas
 
- Python 3.x
- NumPy
- Matplotlib

## Cómo ejecutar
 
1. Clona el repositorio.
2. Instala las dependencias:
```bash
   pip install numpy matplotlib jupyter
```
3. Abre `stellar_luminosity_hands_on.ipynb` con Jupyter (o VS Code) y ejecuta
   todas las celdas en orden (`Run All`).


## Resultado principal
 
El modelo polinómico (usando `mass` y `mass²`) ajusta la relación real de
forma mucho más precisa que el modelo lineal (costo final ≈ 0.32 vs ≈ 9.80),
ya que la luminosidad estelar crece de forma no lineal con la masa. Sin
embargo, al extrapolar fuera del rango observado (mass = 5.0), ambos modelos
divergen fuertemente entre sí, mostrando que un mejor ajuste dentro del rango
de datos no garantiza predicciones confiables fuera de él.