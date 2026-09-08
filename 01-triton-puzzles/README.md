# 01 · Triton Puzzles

Los 12 puzzles de [Triton-Puzzles-Lite](https://github.com/SiriusNEO/Triton-Puzzles-Lite),
resueltos en el intérprete de Triton (CPU, Kaggle, sin GPU).

```bash
git clone https://github.com/SiriusNEO/Triton-Puzzles-Lite
cd Triton-Puzzles-Lite
TRITON_INTERPRET=1 python3 puzzles.py -p 1
```

| Puzzle | Concepto | Día | Estado |
|---|---|---|---|
| 1 Constant Add | grid, program_id | D1 | |
| 2 Constant Add Block | bloques y masking | D1 | |
| 3 Outer Vector Add | indexado 2D | D2 | |
| 4 Outer Vector Add Block | bloques 2D | D2 | |
| 5 Fused Outer Multiplication | fusión | D3 | |
| 6 Fused Outer Mult Backward | fusión en backward | D3 | |
| 7 Long Sum | reducción por bloques | D4 | |
| 8 Long Softmax | reducción + estabilidad numérica | D4 | |
| 9 Simple FlashAttention | online softmax | D5 | |
| 10 Conv 2D | ventanas y bordes | D6 | |
| 11 Matmul | tiling y acumulador | D6 | |
| 12 Quantized Matmul | packing y ancho de banda | D7 | |

Teoría del puzzle 9: `cur-14-flashattention` §2, en la bóveda.
