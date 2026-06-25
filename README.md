# Rahul Kadam

Early-career software engineer working across ML systems, backend infrastructure, performance engineering, and research software.

I build the systems around ML work: benchmark ingestion, reproducible experiments, distributed-training instrumentation, evaluation metrics, numerical pipelines, and backend services that make results easier to trust.

NYU Tandon MS Computer Engineering, 2025. Brooklyn, NY. Open to early-career ML systems, backend, infrastructure, and research-software roles. Willing to relocate.

## What I Build

**ML systems and distributed training**

Fixed-work benchmark protocols, PyTorch/DeepSpeed runs, Slurm launchers, NCCL/Nsight profiling, throughput and step-time analysis, provenance logging.

**Backend and data infrastructure**

FastAPI services, PostgreSQL schemas, Redis-backed workers, async derived metrics, Dockerized demos, migrations, REST APIs, testable data models.

**Scientific and research software**

MRI reconstruction and sampling pipelines, MATLAB-to-Python/PyTorch reimplementation, numerical parity checks, NRMSE/SSIM evaluation, reproducible artifacts.

**Systems and performance engineering**

C++ systems projects, Linux tooling, CI/regression harnesses, profiler-guided debugging, structured run artifacts.

## Selected Work

### [BASS-Python](https://github.com/kadamrahul18/BASS-python)

Python/NumPy and optional PyTorch implementation of Bias Accelerated Subset Selection for learning parallel MRI sampling masks.

- Core technology: NumPy, PyTorch, SENSE-CG reconstruction, complex MRI arrays, NRMSE/SSIM metrics, pytest.
- What I built: BASS sampling loop, epsilon/r heuristic maps, add/remove proposals, center constraints, accept/reject logic, multi-slice execution, artifact generation, and synthetic tests.
- Verify: README separates paper-reported results from repository evidence and provides tests that run without private MRI data.

### [GPT2-Optimization](https://github.com/kadamrahul18/GPT2-Optimization)

Reproducible GPT-2 distributed-training benchmark harness on NYU Big Purple.

- Core technology: PyTorch, DeepSpeed ZeRO-1, Slurm, NCCL, NVTX, Nsight Systems, V100 GPUs.
- What I built: fixed-work launch workflow, benchmark/profiling modes, provenance-rich `training_metrics.json`, NCCL/Nsight artifact capture, scaling/report utilities, tests.
- Verify: checked-in artifacts document the 8-GPU A/B run and profiling context, with caveats kept in the README.

### [Benchmark Results Service](https://github.com/kadamrahul18/benchmark-results-service)

Backend service for ingesting ML benchmark runs and computing derived scaling metrics asynchronously.

- Core technology: FastAPI, PostgreSQL, Redis, Alembic, Docker Compose, pytest, GitHub Actions.
- What I built: REST ingestion API, normalized run schema plus raw JSON retention, Redis worker, derived-metric pipeline, deterministic baseline selection, `/compare`, Docker demo, CI smoke test.
- Verify: `make docker-up` and `make demo` run the local end-to-end path.

### [Opik LLM Evaluation SDK PR #1006](https://github.com/comet-ml/opik/pull/1006)

Merged open-source contribution adding BLEU metrics to Comet ML's Opik SDK.

- Core technology: Python, NLTK BLEU APIs, pytest, SDK documentation.
- What I built: SentenceBLEU and CorpusBLEU metrics, shared validation/smoothing logic, tests for edge cases, docs, and public exports.
- Verify: public PR shows review feedback, requested refactors, approval, and merge.

### [MIPS Pipelined Simulator](https://github.com/CSA-Labs/mips-pipelined)

Five-stage MIPS pipeline simulator in C++ with hazard detection, forwarding, branch handling, and regression traces.

- Core technology: C++, Makefile, simulator traces, golden-output tests.
- Verify: `make test` runs the regression harness against expected register, memory, and state outputs.

### [Brain Tumor Segmentation Baseline](https://github.com/kadamrahul18/Brain-Tumor-Seg)

Medical-imaging training/evaluation baseline with 3D segmentation, metric artifacts, and smoke tests.

- Core technology: Python, MONAI 3D U-Net workflow, Dice metrics, Docker, CI.
- Verify: README and checked-in artifacts document training/evaluation outputs and smoke tests.

## Experience Snapshot

**NYU Langone Health, CAI2R Lab**

Research Software Engineer Intern, fixed-term research project.

- Reimplemented MRI reconstruction and sampling code from MATLAB into Python/PyTorch.
- Added parity checks for SENSE reconstruction outputs.
- Built evaluation around k-space NRMSE, image NRMSE, and SSIM.
- Worked with CUDA-backed experiments and reproducible research artifacts.

## Open Source

**Comet ML Opik SDK**

Merged PR: [Implemented BLEU score, unit tests, and documentation](https://github.com/comet-ml/opik/pull/1006)

The contribution added evaluation metrics that fit the existing SDK design, went through maintainer review, changed from a custom BLEU implementation to NLTK-backed APIs, split into SentenceBLEU and CorpusBLEU, and landed with tests/docs/public exports.

## Technical Toolkit

- Languages: Python, C++, Bash, SQL.
- ML and numerical computing: PyTorch, DeepSpeed, AMP, NumPy, SciPy, MONAI, TensorBoard.
- Distributed and performance tools: Slurm, NCCL, CUDA, NVTX, Nsight Systems, Linux.
- Backend and data: FastAPI, REST APIs, PostgreSQL, Redis, Alembic, Docker Compose.
- Testing and delivery: pytest, GitHub Actions, ruff, Makefiles, reproducible demos.

## Contact

- LinkedIn: https://www.linkedin.com/in/rahul-kadam6399
- GitHub: https://github.com/kadamrahul18
