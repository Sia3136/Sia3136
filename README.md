# Siya Rozani

<p align="left">
  <a href="https://www.linkedin.com/in/siya-rozani-9889592a1" target="_blank"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white" /></a>
  <a href="https://mail.google.com/mail/?view=cm&fs=1&to=siarozani3136@gmail.com" target="_blank"><img src="https://img.shields.io/badge/Email-EA4335?style=flat-square&logo=gmail&logoColor=white" /></a>
  <a href="https://gradientsandgroundtruth.hashnode.dev" target="_blank"><img src="https://img.shields.io/badge/Hashnode-2962FF?style=flat-square&logo=hashnode&logoColor=white" /></a>
  <a href="https://orcid.org/0009-0005-5502-1997" target="_blank"><img src="https://img.shields.io/badge/ORCID-A6CE39?style=flat-square&logo=orcid&logoColor=white" /></a>
  <a href="https://dribbble.com/siarozani3136" target="_blank"><img src="https://img.shields.io/badge/Dribbble-EA4C89?style=flat-square&logo=dribbble&logoColor=white" /></a>
  <a href="https://www.behance.net/siyarozani" target="_blank"><img src="https://img.shields.io/badge/Behance-1769FF?style=flat-square&logo=behance&logoColor=white" /></a>
  <img src="https://komarev.com/ghpvc/?username=Sia3136&label=Views&color=555555&style=flat-square" />
</p>

I turn ideas into working, scalable products — across **ML, DL, LLMs and full-stack systems**.  
From implementing transformer architectures in raw PyTorch and fine-tuning domain models to shipping real-time backends (`FastAPI`, `Redis`, `WebSockets`) and production web apps (`Next.js`, `PostgreSQL`), I build across the full lifecycle from problem framing to deployment.

<sub><i>Open to AI/ML, Deep Learning & Systems/Software Engineering internships, as well as freelance or contract work.</i></sub>

---

## Featured Projects

### Tiny-Shakespeare Decoder-Only Transformer — *From Scratch in PyTorch*
- Built a **16,736-parameter Pre-LN Decoder-Only Transformer** using raw `nn.Embedding`, `nn.Linear`, and `nn.LayerNorm` (zero `nn.Transformer` abstractions) over a **1.11M-character** corpus (`65`-char vocab, `block_size=32`, `AdamW`).
- Hand-coded scaled dot-product self-attention, upper-triangular `-∞` causal masking, residual highways, and a 4× expanded GELU FFN (`8,352` params).
- Dropped validation perplexity from **65.00 → 10.05** (`val_loss 4.17 → 2.31`) in 5 epochs and documented the full tensor-shape and gradient math breakdown.  
**Links:** [Repository](https://github.com/Sia3136/Tiny-Shakespeare-Decoder-Only-Transformer-Language-Model) · [Hashnode Blog](https://gradientsandgroundtruth.hashnode.dev/building-a-decoder-only-transformer-from-scratch-a-tiny-shakespeare-experiment)

### ViewX — *Real-Time AI Surveillance & Proctoring (Top 6 — DrishtiAI Hackathon)*
- Engineered a multi-camera CV pipeline turning passive RTSP/MJPEG streams into real-time anomaly alerts at **~30ms end-to-end frame latency (30+ FPS)**.
- Combined `CLAHE` low-light normalization, `YOLOv8s`, and `ByteTrack` identity persistence with a scale-invariant **Dual-Triangle Sight Tracker** (gaze estimation without eye-trackers) and **invigilator coordinate suppression** to eliminate false positives.
- Decoupled edge workers from `FastAPI` + `PostgreSQL` via `Redis Pub/Sub` and `WebSockets`, backed by `Groq` explainability logs and `pytest` false-positive regression tests.  
**Links:** [Repository](https://github.com/Sia3136/ViewX)

### BidCraft — *Full-Stack Creator Marketplace (Live in Production)*
- Built and deployed a 3-tier marketplace (`Next.js 16`, `Express`, `PostgreSQL`, `Upstash Redis`) supporting **fixed-price checkout, live auctions, and private offer negotiation** across 9 API domains.
- Synchronized live auction clocks via `Socket.io`, automated transactional winner settlement with `node-cron`, and secured payments with webhook-verified `Razorpay` escrow, `15m/7d` rotating `httpOnly` JWTs, and Redis rate limiting.
- Hardened mutating endpoints with `Joi` schemas, parameterized `pg` queries, and `Jest` + `Supertest` integration tests, paired with a custom end-to-end UI design.  
**Links:** [Repository](https://github.com/Sia3136/BidCraft) · [Live App](https://bid-craft-nine.vercel.app) · [Hashnode Blog](https://gradientsandgroundtruth.hashnode.dev/bidcraft-building-trust-into-a-creator-marketplace) · [Dribbble](https://dribbble.com/shots/27878056-BidCraft-Where-Indian-Craft-Meets-Honest-Commerce)

### CodeShieldAI — *Hybrid Code Vulnerability Scanner*
- Built a hybrid static-plus-neural vulnerability scanner combining fine-tuned `GraphCodeBERT` and `CodeBERT` with a deterministic **8-language rule engine** (`Python`, `Java`, `C`, `C++`, `JS/TS`, `PHP`, `C#`, `SQL`).
- Fine-tuned models on **~50,000 samples (~33k vulnerable, ~17k safe)** merged across 6 benchmarks (`DiverseVul`, `Devign`, `ReVeal`, `BigVul`, `CrossVul`, `CVEfixes`), then engineered **boost/rollback scoring** so high-risk static sinks override uncertain ML predictions.
- Delivers GitHub repo/file scanning, side-by-side GraphCodeBERT vs. CodeBERT benchmarking, MongoDB analytics, and exportable JSON/PDF remediation reports.  
**Links:** [Repository](https://github.com/Sia3136/CodeShieldAI) · [Demo Video](https://drive.google.com/drive/folders/1g2O0wYeAbk-KJthrp4tVReRFcjo5Tw2M?usp=sharing)

---

## Engineering Stack

| Area | Tools | Applied In |
| :--- | :--- | :--- |
| **ML, DL & LLMs** | `PyTorch`, `Hugging Face`, `Transformers`, `YOLOv8`, `ByteTrack`, `OpenCV`, `Scikit-learn` | From-scratch transformers, fine-tuning CodeBERT/GraphCodeBERT, 30+ FPS edge CV |
| **Backend & Systems** | `FastAPI`, `Node.js`, `Express`, `PostgreSQL`, `Redis`, `MongoDB`, `Socket.io`, `WebSockets` | Real-time pub/sub alert streams, transactional escrow, rate-limited REST APIs |
| **Frontend & Design** | `Next.js`, `React`, `TypeScript`, `Tailwind CSS`, `Figma` | Production app routing, state management (`Zustand`/`SWR`), UI/UX design systems |
| **Infra & Quality** | `Docker`, `Docker Compose`, `Git`, `pytest`, `Jest`, `Supertest`, `Vercel`, `Render` | Multi-service containerization, automated unit/integration testing, cloud deployment |

---

## GitHub Activity

<p align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com?user=Sia3136&theme=tokyonight&hide_border=true" />
</p>
