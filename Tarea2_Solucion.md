# Estadística para Ciencia de los Datos — Tarea #2 (Solución)

_Generado automáticamente el 2025-08-16 03:04:40_

**Metodología**: Para cada variable cuantitativa seleccionada se ajustaron varias distribuciones candidatas (Normal, Lognormal, Gamma, Exponencial) mediante máxima verosimilitud. Se eligió la candidata con **AIC** más bajo y se validó con la **prueba KS** (α = 0.05). Se incluye histograma con la PDF ajustada, parámetros estimados, estadístico KS y decisión.

## carat

- **Distribución propuesta**: `gamma`

- **Parámetros (shape..., loc, scale)**: `(1.22294, 0.239068, 0.449233)`

- **KS**: estadístico = `0.0708`, p-valor = `0.257` → **No rechazar** H₀ a α = 0.05

- **Justificación**: Los datos son positivos con sesgo a la derecha; Gamma es flexible para colas derechas y tasas. Criterio de selección: menor AIC. Comparativa AIC → gamma: AIC=161.63, expon: AIC=163.74, lognorm: AIC=167.81, norm: AIC=287.25.

- **Figura**: /mnt/data/tarea2_output/carat_fit.png

## price

- **Distribución propuesta**: `gamma`

- **Parámetros (shape..., loc, scale)**: `(0.733125, 394, 4736.51)`

- **KS**: estadístico = `0.0584`, p-valor = `0.4853` → **No rechazar** H₀ a α = 0.05

- **Justificación**: Los datos son positivos con sesgo a la derecha; Gamma es flexible para colas derechas y tasas. Criterio de selección: menor AIC. Comparativa AIC → gamma: AIC=3629.94, lognorm: AIC=3650.02, expon: AIC=3651.53, norm: AIC=3876.50.

- **Figura**: /mnt/data/tarea2_output/price_fit.png

## depth

- **Distribución propuesta**: `norm`

- **Parámetros (shape..., loc, scale)**: `(61.788, 1.42139)`

- **KS**: estadístico = `0.0774`, p-valor = `0.1723` → **No rechazar** H₀ a α = 0.05

- **Justificación**: La forma de la distribución es aproximadamente simétrica con una sola moda; por ello, Normal suele ser adecuada. Criterio de selección: menor AIC. Comparativa AIC → norm: AIC=712.23, lognorm: AIC=714.23, gamma: AIC=716.06, expon: AIC=1038.71.

- **Figura**: /mnt/data/tarea2_output/depth_fit.png

## x

- **Distribución propuesta**: `gamma`

- **Parámetros (shape..., loc, scale)**: `(1.92386, 4.0061, 0.882253)`

- **KS**: estadístico = `0.0806`, p-valor = `0.1404` → **No rechazar** H₀ a α = 0.05

- **Justificación**: Los datos son positivos con sesgo a la derecha; Gamma es flexible para colas derechas y tasas. Criterio de selección: menor AIC. Comparativa AIC → gamma: AIC=575.68, lognorm: AIC=587.13, expon: AIC=607.56, norm: AIC=616.97.

- **Figura**: /mnt/data/tarea2_output/x_fit.png
