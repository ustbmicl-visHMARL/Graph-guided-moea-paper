# Graph-guided-moea-paper

昌琦的"基于图引导的多目标进化学习"论文（需合作修改）。

**Graph-Guided Heterogeneous Dual-Population Evolution for Multi-Objective
Flexible Job Shop Scheduling** — targeting IJAMT (Springer `sn-jnl` template).

## Contents
- `main.tex` — manuscript source
- `main.pdf` — compiled paper
- `references.bib` — bibliography
- `sn-jnl.cls`, `sn-mathphys-num.bst` — Springer Nature journal template
- `images/` — figures

## Build
```bash
pdflatex main.tex
bibtex main
pdflatex main.tex
pdflatex main.tex
```

## Method
A GNN dispatching-rule prior learner feeds a heterogeneous dual-population
NSGA-II (breadth-oriented MP + core-focused EP) coupled by bidirectional
exchange and an adaptive mixed-EP evolution strategy (GNN-HDPCEA-AME) for
three-objective FJSP (makespan, maximum machine load, total load).
