<div align="center">

# Tejas S

**AI Engineer · Computer vision, LLM inference and industrial AI**

I take machine learning systems from research to production, and I measure them honestly on the way.

Bengaluru, India · [LinkedIn](https://www.linkedin.com/in/tejas-s-57298325a/) · s7.tejas@gmail.com

</div>

---

### About

Most recently I built the computer vision engine behind automated match analytics at **The Clutch Sports**: data labelling, model training, multi-player tracking, court calibration and event detection across four sports, with the first sport shipped to production. Before that I worked on ADAS perception at Dots Autonomous, aerospace sensing at CSIR-NAL, and test automation for space-grade electronics at Spacechips.

On my own time I build open-source systems end to end, from the model to the server to the security review, and I evaluate them the way a research team would: held-out data, strong baselines, pre-registered experiments where it matters, and negative results reported as they are.

### Now building: FreeWidth

<a href="https://github.com/Tejascodz/Freewidth"><img src="https://raw.githubusercontent.com/Tejascodz/Freewidth/main/docs/figures/hero.png" width="100%" alt="FreeWidth: wall time versus parallel samples on a T4, and accuracy versus latency on GSM8K"></a>

On a single-user GPU, several LLM samples cost almost the same wall time as one, up to a limit set by the model and the hardware. [**FreeWidth**](https://github.com/Tejascodz/Freewidth) measures that limit on each GPU and builds a two-GPU small-to-large model ladder around it. A 0.8B model samples in parallel and stops early once the answers agree, while a 4B model on the second GPU checks each answer in a single forward pass.

<table>
<tr>
<td align="center" width="33%"><b>1.9×</b><br><sub>lower median latency</sub></td>
<td align="center" width="33%"><b>44%</b><br><sub>less energy per question</sub></td>
<td align="center" width="33%"><b>93.7% vs 95.7%</b><br><sub>accuracy, not significant</sub></td>
</tr>
</table>

<sub>Compared with the 4B model alone on 300 GSM8K problems, using two free Kaggle T4s. The gap is not statistically significant (Holm-corrected p = 0.21), which does not prove equivalence; 90th-percentile latency is higher (74.6 s vs 62.0 s), and a same-session confirmation is still to run.</sub>

### Selected work

| Project | Area | Result |
|---|---|---|
| [**Axon**](https://github.com/Tejascodz/Axon) | Retrieval and RAG | A production RAG system built from scratch: hybrid ColBERT + BM25 search, condition-aware re-ranking and multi-hop retrieval. HotpotQA both-gold@5 from 0.70 to 0.88; prompt-injection success from 5% to 0.25% on attacks no detector was tuned on; zero cross-tenant results in 4,400 hostile queries. |
| [**Industrial AI Guardian**](https://github.com/Tejascodz/industrial-ai-guardian) | Industrial AI | Tells a failing transmitter apart from a real process fault, a regime change or a cyber attack on a closed-loop Tennessee Eastman plant. Detects 94% of events against 52 to 55% for limit-check and PCA baselines, names the faulty transmitter 79% of the time, and catches all 42 attacks. |
| [**Pramana**](https://github.com/Tejascodz/pramana) | AI assurance | Audits ML models, LLM apps and agents and seals the evidence in a hash-chained pack mapped to NIST AI RMF, ISO/IEC 42001 and the EU AI Act. Guardrails cut attack success from 21% to 1.3% over 1,000+ live calls in four languages; reproduces ProPublica's COMPAS error-rate gap within 3 points. |
| [**Drishti**](https://github.com/Tejascodz/drishti) | Computer vision | Number plate recognition for Indian roads and free-flow tolling. YOLO26 plate detector at 96.1% recall and 97.5% precision, with format-aware OCR and multi-frame fusion. |
| [**AI Terrain Rover**](https://github.com/Tejascodz/AI-Based-Rough-Terrain-Rover-for-Search-Reconnaissance) | Robotics | Six-wheel rocker-bogie rover with LiDAR terrain mapping and terrain segmentation, built in a team of four. Presented at CICCS-25; Rank 11 of 1,054 teams across SAARC. |
| [**OpenRoad-Autonomy**](https://github.com/Tejascodz/OpenRoad-Autonomy) | Planning | Delivery robot fleet on real OpenStreetMap roads with ALT, A\*, D\* Lite and Dijkstra planning, battery-aware dispatch and a hardened control API. |

### Experience

| Role | Company | Year | Focus |
|---|---|---|---|
| AI Engineer | The Clutch Sports | 2026 | Multi-sport video analytics; ball tracking at 98% F1, court segmentation at 99%+ mAP50 |
| AI Engineering Intern | Dots Autonomous | 2025 | Monocular ADAS for automatic emergency braking: depth, tracking, time-to-collision |
| Research Intern | CSIR-National Aerospace Laboratories | 2025 | Low-cost impact localisation on aerospace composites, 92% within 5 cm |
| Instrumentation Engineer Intern | Spacechips Ltd (UK, remote) | 2024 | Automated testing of space-grade DC-DC converters over SCPI and VISA |

### Toolbox

- **Machine learning:** PyTorch, Hugging Face Transformers, scikit-learn, LoRA fine-tuning, CUDA
- **Computer vision:** OpenCV, YOLO, ONNX Runtime, segmentation, OCR, pose estimation, multi-object tracking, camera calibration
- **LLM systems:** RAG and late-interaction retrieval (ColBERT), vLLM, SGLang, test-time compute, evaluation and red-teaming
- **Production:** Python, C++, FastAPI, Docker, Prometheus, Grafana, GitHub Actions, CodeQL
- **Industrial and embedded:** process monitoring, virtual sensors, OPC UA, IEC 62443, Jetson, STM32, ESP32

### Recognition

- **1st Prize**, ISRO & NSIL Startup Challenge (2024)
- **Rank 11 of 1,054 teams** across SAARC, Vishwakarma Awards (2025)
- **Top 25 nationally**, AICTE Inventors Challenge (2024)
- **Delegate**, Harvard College HPAIR Conference (2026)
