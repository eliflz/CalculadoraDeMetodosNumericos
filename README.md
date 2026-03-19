## 📖 Descripción

**Calculadora De Metodos Numericos** es una API REST académica que permite resolver problemas de **métodos numéricos** enviando una función matemática como texto plano (por ejemplo `x^2 + 3*x`) junto con los parámetros requeridos por cada método.

Actualmente implementa **integración numérica mediante el Método Trapezoidal Compuesto**, que aproxima el valor de una integral definida dividiendo el intervalo `[a, b]` en `n` subintervalos iguales y aplicando la fórmula:
```
I ≈ (h/2) [f(x₀) + 2f(x₁) + 2f(x₂) + ... + 2f(xₙ₋₁) + f(xₙ)]
```

donde `h = (b - a) / n`.

La API no solo devuelve el resultado numérico final, sino también la **tabla completa de iteraciones**, mostrando para cada punto `xᵢ`: el valor evaluado `f(xᵢ)`, el coeficiente aplicado (1 para los extremos, 2 para los puntos intermedios) y el término sumado. Esto permite al usuario entender el procedimiento paso a paso, lo que la hace ideal para entornos educativos.

> ⚠️ Proyecto en desarrollo activo — se agregarán más métodos numéricos próximamente.
