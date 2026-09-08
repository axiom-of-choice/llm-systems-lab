# llm-systems-lab

Four ML systems experiments, measured, over four weeks (Sep 8 to Oct 5 2026).
Goal: move from using frameworks to being able to explain why they run at the speed they do.

Deliberate constraint: 1 hour per day, no local NVIDIA GPU. Kaggle (2×T4, free),
Colab Pro (L4, 10 USD) and nothing else.

| # | Block | Question answered | Status |
|---|---|---|---|
| [01](01-triton-puzzles/) | Triton mechanics | What is a kernel and how do you think in blocks? | in progress |
| [02](02-kernels/) | Measured kernels | Is this kernel memory-bound or compute-bound, and at what % of peak? | pending |
| [03](03-distributed/) | Multi-GPU | Why is scaling efficiency not 1.0? | pending |
| [04](04-inference/) | Distributed inference | Where is the bottleneck in decode with tensor parallel? | pending |

Each experiment follows the same format: what I wanted to improve, what the baseline was, how I measured it,
what changed and why, what generalizes. Without measured numbers, there is no entry.
