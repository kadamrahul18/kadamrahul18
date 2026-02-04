# Rahul Kadam 👋
MS Computer Engineering (NYU). I build **ML systems**: reproducible benchmarks, distributed training + profiling workflows, and small backend tools that make experiments easy to compare and trust.

📍 Jersey City / NYC • Open to early-career roles (ML systems / platform / backend) • Willing to relocate

---

## What I’m good at (in practice)
- **Distributed training + benchmarking:** fixed-work experiments, throughput & step-time measurement, multi-GPU scaling (PyTorch + DeepSpeed/ZeRO)
- **Performance debugging:** NVTX instrumentation, Nsight Systems traces, bottleneck attribution (compute vs comm vs sync)
- **Reproducibility & engineering maturity:** run artifacts, config conventions, CI smoke tests, “one-command demo” repos
- **Systems foundations:** C++ projects, Linux tooling, test harnesses

---

## Proof-of-work (highlighted)
> If you only click two things: the multi-node benchmark harness + the benchmark registry backend.

### 🚀 Featured Projects

| Project | What it is | How to verify fast |
| --- | --- | --- |
| **[GPT-2 Distributed Training Benchmarks](https://github.com/kadamrahul18/GPT2-Optimization)** | Slurm-native, fixed-work GPT-2 training harness scaling to **2 nodes / 8×V100**, with run artifacts + NVTX/Nsight profiling | README has A/B table + run artifact paths. Includes a measured comm-tuning win (**29,971 → 35,807 tokens/s, +19.5%**) at fixed settings. |
| **[Benchmark Results Service](https://github.com/kadamrahul18/benchmark-results-service)** | Containerized **FastAPI + worker** (Postgres/Redis) that ingests benchmark runs and exposes derived comparisons via `/compare` | `make docker-up && make demo` runs end-to-end locally. CI smoke tests included. |
| **[Opik (Comet ML) – Merged PR #1006](https://github.com/comet-ml/opik/pull/1006)** | OSS contribution: BLEU metrics added with tests + docs | External review + merge trail in PR. |
| **[MIPS Pipelined CPU Simulator](https://github.com/CSA-Labs/mips-pipelined)** | Cycle-accurate 5-stage pipeline (hazards + forwarding) in C++ | Verified via regression tests / traces. |
| **[Brain Tumor Segmentation Baseline (MONAI 3D U-Net)]([https://github.com/kadamrahul18/](https://github.com/kadamrahul18/brain-tumor-seg)** | Reproducible training/eval baseline with guardrails (label/ROI checks, metric conventions) | Saved artifacts + Slurm-ready runs for reruns/plots. |

---

## How I build (my default workflow)
- Define a **fixed workload** (so results are comparable)
- Log **run artifacts** (metrics JSON + metadata + “run complete” markers)
- Use **profiling** (NVTX + Nsight) to turn “it’s slow” into a concrete bottleneck
- Ship changes behind **tests/CI** so it’s not just a local experiment

---

## Open source
- Opik (Comet ML): BLEU metrics (NLTK-backed), unit tests, docs → merged upstream  
  👉 https://github.com/comet-ml/opik/pull/1006

---

## Links
- LinkedIn: https://www.linkedin.com/in/rahul-kadam6399
- GitHub: https://github.com/kadamrahul18
