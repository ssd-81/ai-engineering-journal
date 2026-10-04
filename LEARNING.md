# My AI Engineering Path
<!-- Managed by the ai-engineering-from-scratch learning skills.
     Repo: https://github.com/rohitg00/ai-engineering-from-scratch -->

## Mission
Land a solid AI engineering job in Bengaluru. Build practical, real-world
skills that translate directly to opportunities and the ability to work on
genuine problems — not just theory. Pace is steady (~10 h/week) but the
priority is job-readiness, not covering every phase equally.

## Placement
- Date: 2025-01-XX
- Started: 2025-01-XX
- Score: self-selected
- Entry point: Phase 0: Setup & Tooling
- Pace: ~10 h/week

## Path
| Phase | Name | Status | Est. hours |
|-------|------|--------|------------|
| 0 | Setup & Tooling | Do | 14 |
| 1 | Math Foundations | Do | 23 |
| 2 | ML Fundamentals | Do | 21 |
| 3 | Deep Learning Core | Do | 15 |
| 4 | Computer Vision | Do | 27 |
| 5 | NLP — Foundations to Advanced | Do | 30 |
| 6 | Speech & Audio | Do | 18 |
| 7 | Transformers Deep Dive | Do | 14 |
| 8 | Generative AI | Do | 14 |
| 9 | Reinforcement Learning | Do | 13 |
| 10 | LLMs from Scratch | Do | 26 |
| 11 | LLM Engineering | Do | 19 |
| 12 | Multimodal AI | Do | 65 |
| 13 | Tools & Protocols | Do | 43 |
| 14 | Agent Engineering | Do | 55 |
| 15 | Autonomous Systems | Do | 20 |
| 16 | Multi-Agent & Swarms | Do | 28 |
| 17 | Infrastructure & Production | Do | 32 |
| 18 | Ethics, Safety & Alignment | Do | 31 |
| 19 | Capstone Projects | Do | 620 |

**Total: ~1128 hours across all 20 phases.**

For the Bengaluru-job mission, the highest-leverage shortlist when time
gets tight is: 0, 1, 2, 3, 7, 10, 11, 14. Everything else is "do if you
can, skip with no guilt if a deadline hits".

## Progress log
| Date | Lesson | Quiz | Note |
|------|--------|------|------|
| 2025-01-XX | 00/01 Dev Environment | 1/3 | Misread layer-order question; googled GPU check correctly; verified env passes preflight (Python 3.14, Git 2.55). Cloned curriculum to sibling folder `curriculum/`. |
| 2025-01-XX | 00/02 Git and Collaboration | 3/3 | Set up two-repo layout: `ai-engineering-journal` (LEARNING.md) + `ai-engineering-from-scratch` (fork for lesson work). Deleted orphan `curriculum/` clone. Operating rules: journal commits in `journal/`, code artifacts in `fork/`. |
| 2025-01-XX | 00/03 GPU Setup & Cloud | 3/3 | No local GPU (nvidia-smi absent). Set up venv in fork, installed torch CPU + numpy + matplotlib + jupyter. CPU 3000x3000 matmul: 0.339s. Plan: use Google Colab (free T4) when GPU is needed in Phase 3+. NOTE: self-reported gap on 'why GPUs faster' (parallelism, not clock speed) and fp16 rule (derived from hint, not retained). Re-taught both; lesson added to review queue. |

## Review queue
- `phases/00-setup-and-tooling/01-dev-environment` — four-layer env stack: dependency direction (system → pkg mgr → runtime → AI libs) and why standalone installers like `uv`/`rustup` can bootstrap before the runtime.
- `phases/00-setup-and-tooling/03-gpu-setup-and-cloud` — (1) GPU parallelism: thousands of slow cores beat few fast cores for matrix ops; (2) fp16 rule of thumb derivation: 2 bytes/param → VRAM/2 = max params; (3) async GPU: `synchronize()` is the "wait for queue" barrier.
