# 🎧 Visualizador de Delta-Dirac para Archivos WAV

Este programa permite visualizar el "delta" (primera diferencia discreta) de una señal de audio `.wav` usando una interfaz gráfica con `tkinter` y `matplotlib`.
---

## 🎯 ¿Qué hace este programa?

Este visualizador:

1. Permite al usuario **cargar un archivo `.wav`** mediante una ventana gráfica.
2. Extrae las **primeras 30 muestras** del audio.
3. Calcula la **diferencia entre cada muestra y la siguiente** (es decir, el "delta", también llamado diferencia hacia adelante).
4. Muestra una **gráfica tipo "impulso"** (`stem plot`) que representa cómo varía el audio entre muestra y muestra.
5. Todo esto integrado en una **ventana de `tkinter` con `matplotlib` embebido**.

---

## 📊 ¿Qué es un "delta" aquí?

En señales digitales, el delta (o "primera diferencia") entre muestras es una manera sencilla de analizar cómo cambia la señal. Matemáticamente:

```
delta[n] = x[n+1] - x[n]
```

Se usa para:

* Detección de transiciones rápidas (bordes)
* Preprocesamiento de señales
* Aproximación de la derivada discreta

## 🚀 Características

- Interfaz gráfica intuitiva
- Carga archivos `.wav` desde el sistema
- Extrae las primeras 30 muestras del audio
- Calcula las 29 diferencias entre esas muestras (delta)
- Muestra una gráfica tipo **stem** con los valores delta
- Detecta si el audio es estéreo o mono (y toma solo un canal)

---

## 🛠️ Requisitos

- Python 3.7 o superior
- Módulos:

```bash
pip install numpy scipy matplotlib
````

> `tkinter` viene incluido con Python por defecto.
> En Linux puedes instalarlo con:
>
> ```bash
> sudo apt install python3-tk
> ```

---

## 🧪 Uso

1. Ejecuta el script:

   ```bash
   python delta_audio.py
   ```

2. Haz clic en **"Cargar Archivo de Audio"** y selecciona un `.wav`.

3. Observa la gráfica generada con las diferencias entre las primeras 30 muestras.

---

## 📚 Aplicaciones

* Análisis de transitorios o bordes en señales de audio
* Procesamiento digital de señales (DSP)
* Educación en sistemas discretos y audio digital

---

## 👤 Autor

**Dilan Acosta**

---

