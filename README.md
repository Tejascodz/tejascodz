## Tejas S

AI Engineer, computer vision · Bengaluru, India

I build computer vision systems that work on real-world video, from data labelling and model training to
tracking, calibration and production deployment. Most recently at **The Clutch Sports**, where I built the vision
engine behind automated match analytics across four sports. Previously ADAS perception at Dots Autonomous,
aerospace sensing at CSIR-NAL, and test automation for space-grade electronics at Spacechips.

**Currently working on:** [**Axon**](https://github.com/Tejascodz/Axon), a retrieval-augmented generation system
built from scratch and run as a production service. It has hybrid ColBERT + BM25 search with condition-aware
re-ranking, multi-hop retrieval with LLM-written follow-up searches, LLM query expansion, a prompt-injection
classifier and planted-document filters, tenant isolation, live index updates, LLM serving benchmarked on vLLM and
SGLang, and LoRA fine-tuning, deployed with Docker, Prometheus and Grafana, all measured with pre-registered experiments on held-out data.

**Open to work:** AI and computer vision engineering roles in Bengaluru,
Reach me on [LinkedIn](https://www.linkedin.com/in/tejas-s-57298325a/) or at s7.tejas@gmail.com.

### Selected projects

| Project | Description |
|---|---|
| [**Industrial AI Guardian**](https://github.com/Tejascodz/industrial-ai-guardian) | Monitors the transmitters behind an industrial soft sensor and tells a transmitter fault (and which one) apart from a real process fault, a regime change or a data-integrity attack. On a closed-loop Tennessee Eastman simulation it detects 94% of events at 0.29 false alarms per day, against 52 to 55% for limit-check and PCA baselines, names the faulty transmitter in 79% of cases, and detects all 42 replay, freeze and stealth attacks. Encrypted read-only OPC UA link, signed models, tamper-evident audit log and a live control-room HMI. |
| [**AI Terrain Rover**](https://github.com/Tejascodz/AI-Based-Rough-Terrain-Rover-for-Search-Reconnaissance) | Semi-autonomous six-wheel rocker-bogie rover with LiDAR terrain mapping, AI terrain classification and a live telemetry dashboard. Presented at CICCS-25. |
| [**Pramana**](https://github.com/Tejascodz/pramana) | Open-source AI assurance tool that audits ML models, LLM applications and AI agents for fairness, drift, privacy, prompt injection and identity spoofing, and seals the evidence in a signed, hash-chained pack mapped to NIST AI RMF, ISO/IEC 42001 and the EU AI Act. Red-teamed a RAG loan assistant on Llama 3.2 3B over 1,000+ live calls in English, Hindi, Kannada and Tamil, including multi-turn and obfuscated attacks; guardrails cut attack success from 21% to 1.3%. Validated on ProPublica's COMPAS court data, where it reproduces the published racial error-rate gap within 3 points (42.3% vs 22.0% of Black and white defendants who did not reoffend labelled higher risk; published 44.9% vs 23.5%). Tests agents in a honeypot sandbox and through their LangChain or OpenTelemetry logs, audits web chat windows through a real browser, and opens results in an interactive viewer. 450+ tests, CodeQL and build-provenance attestation in CI. |
| [**Axon**](https://github.com/Tejascodz/Axon) | Production RAG system built from scratch on hybrid ColBERT + BM25 search with condition-aware re-ranking. On HotpotQA, both gold passages in the top 5 rise from 0.70 to 0.82 with re-ranking and to 0.88 with a second retrieval hop; LLM-written follow-up searches lift MuSiQue (all supporting passages in the top 10) from 0.38 to 0.53, and LLM query expansion lifts BRIGHT nDCG@10 from 0.16 to 0.26. LoRA fine-tuning of Qwen3-4B adds +18 points exact match and lifts citation recall from 0.48 to 0.81. Guardrails cut prompt-injection success from 10.5% to 0.5%, and a prompt-injection classifier cuts it from 5% to 0.25% on attacks no detector was tuned on; planted false documents go from 21% false answers to 0%; zero cross-tenant results in 4,400 hostile queries. Recall@100 0.96 at 300,000 passages, live index updates 96× faster than rebuilds, 99.8% success under sustained load. vLLM and SGLang benchmarked on T4 GPUs (SGLang 1.8× throughput at 16 concurrent users). Docker, Prometheus and Grafana, security scans and end-to-end tests in CI. Pre-registered experiments and held-out evaluation with confidence intervals and documented negative results. |
| [**OpenRoad-Autonomy**](https://github.com/Tejascodz/OpenRoad-Autonomy) | Delivery robot fleet on real OpenStreetMap roads: ALT, A\*, D\* Lite and Dijkstra planning, velocity-profiled trajectories, battery-aware dispatch and a live control center with a hardened API. |
| [**Drishti**](https://github.com/Tejascodz/drishti) | Number plate recognition for Indian roads and multi-lane free-flow tolling. Trained YOLO26 plate detector (96.1% recall, 97.5% precision), slot OCR with Indian-format decoding, multi-frame fusion and a VLM-assisted review loop. |

### Experience

- **AI Engineer**, The Clutch Sports · 2026
- **AI Engineering Intern**, Dots Autonomous · 2025
- **Research Intern**, CSIR-National Aerospace Laboratories · 2025
- **Automation Engineer Intern**, Spacechips Ltd (UK, remote) · 2024

### Technical focus

Python, C++ · PyTorch, OpenCV, YOLO, ONNX Runtime · detection, segmentation, OCR, pose estimation,
multi-object tracking, camera calibration · LLM evaluation and red-teaming, AI audit (fairness, privacy, NIST AI RMF, EU AI Act), RAG, late-interaction retrieval (ColBERT), LLM serving (vLLM, SGLang), LoRA fine-tuning, FastAPI, Docker, Prometheus, Grafana · process monitoring and fault isolation (virtual sensors, PCA), OPC UA, IEC 62443 · Jetson, STM32, ESP32

### Recognition

- 1st Prize, ISRO & NSIL Startup Challenge (2024)
- Rank 11 of 1,054 teams across SAARC, Vishwakarma Awards (2025)
- Top 25 nationally, AICTE Inventors Challenge (2024)
- Delegate, Harvard College HPAIR Conference (2026)

### Contact

[LinkedIn](https://www.linkedin.com/in/tejas-s-57298325a/) · s7.tejas@gmail.com
