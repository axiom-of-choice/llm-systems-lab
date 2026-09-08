# 01 · Triton Puzzles

The 12 puzzles from [Triton-Puzzles-Lite](https://github.com/SiriusNEO/Triton-Puzzles-Lite), solved in
the Triton interpreter (CPU, no GPU needed).

The harness is vendored here (Apache 2.0, see `NOTICE`), so this directory is self-contained.

- `puzzles.md` is the manual: every puzzle with its diagram of the memory access pattern. Read the
  diagram before writing the kernel. GitHub and Obsidian both render it.
- `puzzles.py` holds the same statements as docstrings, plus the harness you edit.
- `puzzles_ans.py` is deliberately not vendored.

```bash
TRITON_INTERPRET=1 python3 puzzles.py -p 1     # one puzzle
TRITON_INTERPRET=1 python3 puzzles.py -a       # all, stops at the first failure
```

Triton has no macOS wheels, so this runs on Kaggle (CPU session) or in a linux/arm64 container.

| Puzzle | Concept | Day | Status |
|---|---|---|---|
| 1 Constant Add | grid, program_id | D1 | |
| 2 Constant Add Block | blocks and masking | D1 | |
| 3 Outer Vector Add | 2D indexing | D2 | |
| 4 Outer Vector Add Block | 2D blocks | D2 | |
| 5 Fused Outer Multiplication | fusion | D3 | |
| 6 Fused Outer Mult Backward | fusion in backward | D3 | |
| 7 Long Sum | reduction by blocks | D4 | |
| 8 Long Softmax | reduction + numerical stability | D4 | |
| 9 Simple FlashAttention | online softmax | D5 | |
| 10 Conv 2D | windows and borders | D6 | |
| 11 Matmul | tiling and accumulator | D6 | |
| 12 Quantized Matmul | packing and bandwidth | D7 | |

Theory for puzzle 9: `cur-14-flashattention` §2, in the vault.
