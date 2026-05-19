# 🧠 Medical World Models in Healthcare

> A curated survey of **Medical World Models (MWMs)** for simulating patient trajectories, disease progression, medical imaging evolution, and treatment decision-making.
>
> 📌 This repository systematically organizes recent work on world models in medicine, including Electronic Health Records (EHR), medical imaging, physiological systems, multimodal reasoning, and clinical decision support.

---

## 📖 What is a Medical World Model?

A **Medical World Model (MWM)** is a generative and predictive model that learns the dynamics of medical systems.

It models how patient states evolve over time under interventions such as medications, surgeries, radiotherapy, or image-guided procedures.

Compared with traditional predictive models, MWMs explicitly learn:

- **State Representation**: latent representation of patient condition
- **Dynamics Model**: disease progression over time
- **Action Model**: effect of treatments and interventions
- **Reward / Utility Model**: clinical outcomes such as survival, remission, toxicity, or quality of life
- **Planning Module**: simulation-based treatment optimization

### Core Applications

- 🏥 Longitudinal EHR simulation
- 🧬 Disease progression modeling
- 🩻 Medical image forecasting
- ❤️ Physiological system simulation
- 🤖 Clinical decision support
- 🔬 Digital twins
- 💊 Treatment planning

---

## 🗺️ Taxonomy of Medical World Models

```text
Medical World Models
├── Patient State Models
│   ├── EHR trajectory simulation
│   ├── Disease progression
│   └── Risk forecasting
│
├── Medical Imaging Models
│   ├── Tumor growth
│   ├── Organ evolution
│   └── Treatment response
│
├── Physiological Mechanism Models
│   ├── Cardiovascular systems
│   ├── Brain dynamics
│   └── Pharmacokinetics / pharmacodynamics
│
├── Multimodal Models
│   ├── EHR + Imaging
│   ├── EHR + Genomics
│   └── Vision-Language Medical Agents
│
└── Clinical Decision Models
    ├── Treatment planning
    ├── Reinforcement learning
    └── Digital twins
```

---

# 📚 Paper Collection

> The following table lists all 26 papers and resources extracted from the provided document, sorted by publication year in reverse chronological order.

| Year | Title | Venue | Topic | Category | Code |
|------|-------|-------|-------|----------|------|
| 2026 | CLARITY: Medical World Model for Guiding Treatment Decisions by Modeling Context-Aware Disease Trajectories in Latent Space | - | Context-aware disease trajectory modeling | Clinical Decision Making | [Code](https://github.com/DingTianxingjian/CLARITY) |
| 2026 | EHRWorld: A Patient-Centric Medical World Model for Long-Horizon Clinical Trajectories | - | Long-horizon EHR simulation | Patient State Modeling; Clinical Decision Making | - |
| 2026 | MedVersa: A Generalist Foundation Model for Diverse Medical Imaging Tasks | NEJM AI | Generalist medical imaging foundation model | Multimodal Learning; Medical Imaging | - |
| 2026 | CancerLLM: A Large Language Model in Cancer Domain | npj Digital Medicine | Oncology domain language model | Clinical Decision Making; Physiological Mechanism Modeling | [Code](https://github.com/ToneLi/CancerLLM) |
| 2026 | Holistic Evaluation of Large Language Models for Medical Tasks with MedHELM | Nature Medicine | Comprehensive evaluation of medical LLMs | Multimodal Learning | [Code](https://github.com/stanford-crfm/helm) |
| 2025 | Medical World Model | ICCV 2025 | Tumor treatment simulation | Medical Imaging; Clinical Decision Making | [Code](https://github.com/scott-yjyang/MeWM) |
| 2025 | MIRA: Medical Time Series Foundation Model for Real-World Health Data | NeurIPS 2025 | Foundation model for medical time series | Patient State Modeling | [Code](https://github.com/microsoft/MIRA) |
| 2025 | Beyond Generative AI: World Models for Clinical Prediction, Counterfactuals, and Planning | - | Theoretical framework for clinical world models | Multimodal Learning; Physiological Mechanism Modeling; Clinical Decision Making | - |
| 2025 | Medical Digital Twins for Precision Oncology | - | Oncology digital twins | Medical Imaging; Clinical Decision Making | - |
| 2025 | Reinforcement Learning for Adaptive Radiotherapy | - | Adaptive radiotherapy planning | Medical Imaging; Clinical Decision Making | - |
| 2025 | Foundation Models for Clinical Time Series | - | Survey of clinical time-series foundation models | Patient State Modeling | - |
| 2025 | World Models for Healthcare Agents | - | World models for medical agents | Multimodal Learning; Clinical Decision Making | - |
| 2024 | Med-PaLM M | Nature | Multimodal medical foundation model | Multimodal Learning; Clinical Decision Making | - |
| 2024 | LLaVA-Med | NeurIPS Workshop | Medical vision-language model | Multimodal Learning; Medical Imaging | [Code](https://github.com/microsoft/LLaVA-Med) |
| 2024 | BioViL-T | CVPR | Biomedical vision-language foundation model | Multimodal Learning | [Code](https://github.com/microsoft/BioViL) |
| 2024 | Generalist Medical AI (GMAI) | - | General-purpose medical AI framework | Multimodal Learning; Clinical Decision Making | - |
| 2023 | Diffusion Models for Medical Image Generation: A Survey | Medical Image Analysis | Survey of diffusion models in medical imaging | Medical Imaging | - |
| 2023 | Segment Anything Model for Medical Images | Nature Communications | Universal medical image segmentation | Medical Imaging | [Code](https://github.com/bowang-lab/MedSAM) |
| 2022 | RETAIN: Interpretable Predictive Model in Healthcare using Reverse Time Attention | NeurIPS | Interpretable clinical prediction | Patient State Modeling | [Code](https://github.com/mp2893/retain) |
| 2021 | Med-BERT: Pretrained Contextualized Embeddings on Large-Scale Structured EHR Data | NPJ Digital Medicine | EHR pretraining | Patient State Modeling | [Code](https://github.com/ZhiGroup/Med-BERT) |
| 2021 | G-BERT: Pre-training of Graph Augmented Transformers for Medication Recommendation | KDD | Medication recommendation | Patient State Modeling; Clinical Decision Making | [Code](https://github.com/jshang123/G-Bert) |
| 2021 | Neural Ordinary Differential Equations for Continuous-Time Disease Progression | - | Continuous-time disease modeling | Physiological Mechanism Modeling; Patient State Modeling | - |
| 2020 | The Digital Twin to Enable the Vision of Precision Cardiology | European Heart Journal | Cardiovascular digital twins | Patient State Modeling; Physiological Mechanism Modeling | - |
| 2020 | BEHRT: Transformer for Electronic Health Records | Scientific Reports | Transformer modeling for EHR | Patient State Modeling | [Code](https://github.com/deepmedicine/BEHRT) |
| 2019 | A Machine Learning Model to Predict Hepatocellular Carcinoma Response to Transcatheter Arterial Chemoembolization | Radiology: Artificial Intelligence | TACE response prediction | Medical Imaging; Patient State Modeling | - |
| 2018 | The Artificial Intelligence Clinician Learns Optimal Treatment Strategies for Sepsis in Intensive Care | Nature Medicine | Reinforcement learning for sepsis treatment | Multimodal Learning; Clinical Decision Making | - |


# 📑 Comparison Table

| Dimension | Traditional ML | Medical LLMs | Medical World Models |
|------|------|------|------|
| Single-step prediction | ✅ | ✅ | ✅ |
| Long-horizon simulation | ❌ | Limited | ✅ |
| Counterfactual treatment evaluation | ❌ | Limited | ✅ |
| Personalized planning | ❌ | Partial | ✅ |
| Mechanistic modeling | ❌ | ❌ | ✅ |
| Digital twin support | ❌ | ❌ | ✅ |

---


# 🤝 Contributing

Contributions are welcome.

You can help by:

- Adding new papers
- Improving summaries
- Updating benchmarks
- Sharing datasets and code



# ⭐ Star History

If you find this repository useful, please consider giving it a ⭐.



# 📬 Contact

For suggestions and corrections, please open an issue or pull request.
