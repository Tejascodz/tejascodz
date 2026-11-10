## Tejas S

AI Engineer, computer vision · Bengaluru, India

I build computer vision systems that work on real-world video, from data labelling and model training to
tracking, calibration and production deployment. Most recently at **The Clutch Sports**, where I built the vision
engine behind automated match analytics across four sports. Previously ADAS perception at Dots Autonomous,
aerospace sensing at CSIR-NAL, and test automation for space-grade electronics at Spacechips.

**Currently working on:** [**Axon**](https://github.com/Tejascodz/Axon), a retrieval-augmented generation system
built from scratch. It has condition-aware ColBERT re-ranking with per-condition evidence, hybrid search, guardrails
against prompt injection, tenant isolation, LLM serving benchmarked on vLLM and SGLang (time to first token,
inter-token latency, throughput) and LoRA fine-tuning, all measured with pre-registered experiments.

**Open to work:** AI and computer vision engineering roles in Bengaluru, available from November 2026.
Reach me on [LinkedIn](https://www.linkedin.com/in/tejas-s-57298325a/) or at s7.tejas@gmail.com.

### Selected projects

| Project | Description |
|---|---|
| [**Industrial AI Guardian**](https://github.com/Tejascodz/industrial-ai-guardian) | Monitors the transmitters behind an industrial soft sensor and tells a transmitter fault (and which one) apart from a real process fault, a regime change or a data-integrity attack. On a closed-loop Tennessee Eastman simulation it detects 94% of events at 0.29 false alarms per day, against 52 to 55% for limit-check and PCA baselines, names the faulty transmitter in 79% of cases, and detects all 42 replay, freeze and stealth attacks. Encrypted read-only OPC UA link, signed models, tamper-evident audit log and a live control-room HMI. |
| [**AI Terrain Rover**](https://github.com/Tejascodz/AI-Based-Rough-Terrain-Rover-for-Search-Reconnaissance) | Semi-autonomous six-wheel rocker-bogie rover with LiDAR terrain mapping, AI terrain classification and a live telemetry dashboard. Presented at CICCS-25. |
| [**Pramana**](https://github.com/Tejascodz/pramana) | AI assurance tool that tests ML models and LLM applications for fairness, drift, privacy and prompt injection, with evidence mapped to NIST AI RMF, ISO/IEC 42001 and the EU AI Act. |
| [**Axon**](https://github.com/Tejascodz/Axon) | RAG system built from scratch on condition-aware ColBERT re-ranking. Re-ranking raises both-gold-in-top-5 on HotpotQA from 0.70 to 0.82; LoRA fine-tuning of Qwen3-4B adds +18 points exact match and lifts citation recall from 0.48 to 0.81; guardrails cut prompt-injection success from 10.5% to 0.5%, with zero cross-tenant leakage. vLLM and SGLang benchmarked on T4 GPUs (SGLang 1.8× throughput at 16 concurrent users). Pre-registered experiments with confidence intervals and documented negative results. |
| [**OpenRoad-Autonomy**](https://github.com/Tejascodz/OpenRoad-Autonomy) | Delivery robot fleet on real OpenStreetMap roads: ALT, A\*, D\* Lite and Dijkstra planning, velocity-profiled trajectories, battery-aware dispatch and a live control center with a hardened API. |
| [**Drishti**](https://github.com/Tejascodz/drishti) | Number plate recognition for Indian roads and multi-lane free-flow tolling. Trained YOLO26 plate detector (96.1% recall, 97.5% precision), slot OCR with Indian-format decoding, multi-frame fusion and a VLM-assisted review loop. |

### Experience

- **AI Engineer**, The Clutch Sports · 2026
- **AI Engineering Intern**, Dots Autonomous · 2025
- **Research Intern**, CSIR-National Aerospace Laboratories · 2025
- **Automation Engineer Intern**, Spacechips Ltd (UK, remote) · 2024

### Technical focus

Python, C++ · PyTorch, OpenCV, YOLO, ONNX Runtime · detection, segmentation, OCR, pose estimation,
multi-object tracking, camera calibration · LLM evaluation, RAG, late-interaction retrieval (ColBERT), LLM serving (vLLM, SGLang), LoRA fine-tuning · process monitoring and fault isolation (virtual sensors, PCA), OPC UA, IEC 62443 · Jetson, STM32, ESP32

### Recognition

- 1st Prize, ISRO & NSIL Startup Challenge (2024)
- Rank 11 of 1,054 teams across SAARC, Vishwakarma Awards (2025)
- Top 25 nationally, AICTE Inventors Challenge (2024)
- Delegate, Harvard College HPAIR Conference (2026)

### Contact

[LinkedIn](https://www.linkedin.com/in/tejas-s-57298325a/) · s7.tejas@gmail.com
