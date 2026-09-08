# llm-systems-lab

Cuatro experimentos de sistemas de ML, medidos, en cuatro semanas (8 sep a 5 oct 2026).
Objetivo: pasar de usar frameworks a poder explicar por qué van a la velocidad que van.

Restricción deliberada: 1 hora al día, sin GPU NVIDIA local. Kaggle (2×T4, gratis),
Colab Pro (L4, 10 USD) y nada más.

| # | Semana | Pregunta que responde | Estado |
|---|---|---|---|
| [01](01-triton-puzzles/) | Triton, la mecánica | ¿Qué es un kernel y cómo se piensa por bloques? | en curso |
| [02](02-kernels/) | Kernels medidos | ¿Este kernel es memory-bound o compute-bound, y a qué % del techo está? | pendiente |
| [03](03-distributed/) | Multi-GPU | ¿Por qué la eficiencia de escalado no es 1.0? | pendiente |
| [04](04-inference/) | Inferencia distribuida | ¿Dónde está el cuello de botella en decode con tensor parallel? | pendiente |

Cada experimento sigue el mismo formato: qué quería mejorar, cuál era el baseline, cómo lo medí,
qué cambió y por qué, qué generaliza. Sin número medido no hay entrada.
