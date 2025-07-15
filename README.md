# 🧮 Scoring de Solvencia para Emisores de Obligaciones Negociables (ONs) - Argentina

Este proyecto está diseñado para evaluar la **solvencia financiera de empresas emisoras de Obligaciones Negociables (ONs)** en el mercado de capitales argentino. Se calcula una **nota ponderada** para cada emisor, a partir de ratios financieros clave, con el objetivo de facilitar un análisis crediticio estructurado y cuantitativo.

## 🎯 Objetivo

El análisis busca responder una sola pregunta:

> ¿Qué tan solvente es cada empresa emisora de ONs, según sus indicadores financieros más relevantes?

Este sistema de scoring permite **ordenar emisores según su calidad crediticia**, y así tomar decisiones más fundamentadas a la hora de invertir en renta fija corporativa.

---

## 🧠 ¿Cómo funciona?

Se parte de un archivo de entrada con los **ratios financieros de cada empresa emisora**. Luego:

1. Cada ratio es **normalizado** para que todos sean comparables.
2. Se aplica un **peso específico** a cada ratio según su relevancia.
3. Se calcula una **nota final ponderada** que resume la solvencia de cada emisor.

### 📊 Ratios utilizados

Los siguientes ratios fueron elegidos por su capacidad de capturar distintos aspectos de la salud financiera de una empresa:

- **Pasivo Corriente / Activo Corriente** → mide liquidez de corto plazo.
- **Pasivo / Activo** → muestra el apalancamiento total.
- **Efectivo / Pasivo Corriente** → liquidez inmediata.
- **Apalancamiento** → relación de deuda respecto al patrimonio.
- **EBITDA / Intereses** → cobertura de intereses, capacidad de repago.
- **Deuda Financiera Neta / EBITDA** → años necesarios para pagar deuda con resultados operativos.
- **Deuda Financiera Neta / Patrimonio Neto** → solvencia estructural.

Cada ratio puede ser ponderado con distinta importancia (vos mismo lo ajustás en el código).
