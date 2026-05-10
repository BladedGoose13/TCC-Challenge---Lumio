
# SROI-LUMIO

**Índice de Retorno Social de Inversión**  
Documento técnico know-how · XIGNUX Gestión ESG · 2026

---

![License](https://img.shields.io/badge/license-CC_BY--NC--ND_4.0-red)
![Status](https://img.shields.io/badge/status-experimental-orange)
![Framework](https://img.shields.io/badge/framework-ESG%20%2F%20SROI-green)

---

## Technical Document

📄 **Read the full technical whitepaper here:**

[![Open PDF](https://img.shields.io/badge/Open-Know--How.pdf-blue?style=for-the-badge)](./Know-How.pdf)

---

## ¿Qué es SROI-LUMIO?

SROI-LUMIO es un modelo matemático propietario para medir y comparar el retorno social de proyectos de impacto. A diferencia del SROI clásico, produce un índice adimensional en el intervalo [0, 2) mediante una transformación logarítmica que codifica rendimientos marginales decrecientes, eliminando la necesidad de monetizar subjetivamente el impacto social.

| Valor | Clasificación |
|-------|--------------|
| (0, 0.5) | Crítico |
| [0.5, 1) | Bajo desempeño |
| = 1 | Punto de equilibrio |
| (1, 1.5) | Rentable |
| [1.5, 2) | Alto impacto |

---

## Componentes del modelo

El índice se construye sobre cuatro piezas que convergen en un retorno ponderado efectivo `u`, el cual pasa por la transformación logarítmica final.

| Componente | Símbolo | Descripción |
|-----------|---------|-------------|
| Perspectiva Integral | PS | Cumplimiento de metas sociales, ambientales e infraestructura, ajustado por causalidad (FA) |
| Factor de Ajuste Causal | FA | Descuenta deadweight, attribution, displacement y drop-off |
| Factor de Colaboración | FC | Amplifica el índice según participación de socios comerciales |
| Factor de Fricción Logística | FL | Penaliza costos que no generan valor directo |
| Retorno Monetario | RM | Cumplimiento normalizado de la meta financiera |

**Ecuación central:**

$$\text{SROI-LUMIO} = \frac{2\ln(1+u)}{\ln(1+u) + \ln 2}$$

$$u = \bigl[\alpha \cdot \text{PS} + \gamma \cdot \text{RM}\bigr] \cdot \text{FL} \cdot \text{FC}$$

---

## Archivos en este directorio

| Archivo | Descripción |
|---------|-------------|
| `Descripción.md` | Resumen ejecutivo del modelo y sus variables |
| `Know-How.pdf` | Documento técnico completo con derivaciones, ejemplos numéricos, Monte Carlo y optimización por knapsack |

---

## Autores

| Nombre | Carrera |
|--------|---------|
| Maximilien Tragarz Quintana | Ingeniería Física (IFI) |
| Agatha Adaluz Liewald Suarez | Ingeniería Física (IFI) |
| Karla Yveth Alemán Pastrana | Inteligencia de Negocios (LIT) |

---

## Licencia

Distribuido bajo **SROI-LUMIO Model License**.  
Uso libre para fines académicos y de investigación con atribución a los autores.  
Todo uso comercial requiere autorización escrita de los autores.  
Ver archivo [`LICENSE`](../../LICENSE) en la raíz del repositorio.

© 2026 SROI-LUMIO
