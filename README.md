# Hi, I'm Rahul Kadam 👋

MS Computer Engineering @ NYU. I work on ML systems: distributed training benchmarks, evaluation tooling, and reproducible experimentation.

### 🔭 Engineering Focus
* **Distributed Training & Benchmarking:** fixed-work experiments, throughput/step-time measurement, multi-GPU scaling (PyTorch + DeepSpeed/ZeRO)
* **Systems Foundations:** C++ projects (cycle-accurate simulators), Linux tooling, test harnesses
* **Open Source:** Contributed to Opik (Comet ML) Python SDK — merged PR with unit tests + docs

### 🚀 Highlighted Projects

| Project | Tech Stack | Evidence / Impact |
| :--- | :--- | :--- |
| **[Distributed LLM Training Benchmarks](https://github.com/kadamrahul18/GPT2-Optimization)** | PyTorch, DeepSpeed, Slurm | Fixed-work multi-GPU benchmarking for GPT-2 (124M); tokens/sec scaling and run artifacts for reproducibility. |
| **[MIPS Processor Simulator](https://github.com/CSA-Labs/mips-pipelined)** | C++, Linux, Make | Cycle-accurate 5-stage pipeline simulator with hazard detection + forwarding; verified via regression tests / traces. |
| **[Opik LLM Eval Platform (Merged PR #1006)](https://github.com/comet-ml/opik/pull/1006)** | Python, Pytest, Docs | Added SentenceBLEU/CorpusBLEU metrics (NLTK-backed) + unit tests + docs; exported via `opik.evaluation.metrics`. |
| **[Brain Tumor Segmentation Baseline (MONAI 3D U-Net)](https://github.com/kadamrahul18/Classification-of-MRI-images-for-Brain-Tumor-Using-Convolutional-Neural-Networks)** | PyTorch, MONAI, Linux, Slurm | Reproducible training/eval pipeline on MSD Task01 with guardrails (ROI/label checks, metric conventions) and saved artifacts for reruns/plots. |

### 🛠️ Tech Stack
* **Systems:** Python, C++, Linux, Bash
* **ML Systems:** PyTorch, DeepSpeed (ZeRO), testing (pytest), experiment reproducibility (configs/artifacts)
* **Tooling:** Git, Docker

[<img src="https://img.shields.io/badge/linkedin-%230077B5.svg?&style=for-the-badge&logo=linkedin&logoColor=white" />](https://www.linkedin.com/in/rahul-kadam6399/)
