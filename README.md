# Sana Firdouse

**Computer Science | Artificial Intelligence, Machine Learning & Trustworthy Autonomous Systems**

I develop and evaluate research-oriented software prototypes across machine learning, deep learning, multimodal modelling, and the security of tool-using AI agents. My work focuses on making systems measurable and understandable: defining the task, choosing appropriate baselines, testing assumptions, documenting limitations, and avoiding claims that the evidence does not support.

## Research areas

- **Machine learning and statistical evaluation:** supervised learning, model comparison, validation design, error analysis, and reproducible experiments.
- **Deep learning:** neural-network baselines and representation learning with PyTorch and TensorFlow/Keras.
- **Computer vision and multimodal learning:** image-derived features, multimodal feature fusion, and combining imaging-related, clinical/temporal, and wearable-style numerical data.
- **Longitudinal and healthcare machine learning:** next-visit prediction experiments, missing-modality analysis, uncertainty estimation, and careful separation of synthetic demonstrations from clinical evidence.
- **Trustworthy AI and LLM-agent security:** provenance-aware processing, capability restrictions, policy evaluation, continuous authorization, and controls at the boundary where an agent attempts an action.
- **Cybersecurity and secure systems:** threat modelling, least privilege, auditability, input and boundary validation, and security evaluation of agent integrations.
- **Natural language processing:** text-processing methods and NLP tooling.

These are areas of technical work and research interest; the scope and maturity of each implementation are described in its repository.

## Selected projects

### 1. PACA++ — authorization and security for LLM agents

PACA++ explores how authorization decisions can remain bound to an intended action, target, policy, and context when an AI agent attempts a consequential operation.

- [PACA-Plus-Plus-New](https://github.com/sanafirdouse2323-glitch/PACA-Plus-Plus-New) — a Python reference-monitor prototype with provenance labels, task- and target-bound capabilities, policy rules, manifest pinning, delegation controls, effect-token checks, deterministic attack simulations, and a limited AgentDojo integration.
- [PACA-Plus-Plus](https://github.com/sanafirdouse2323-glitch/PACA-Plus-Plus) — a related authorization/compiler and service research scaffold. Its compiler supports only a documented policy subset; it is not a complete ALFA/UCON+ compiler.

**Evidence boundary:** the attack scenarios in PACA-Plus-Plus-New are author-written deterministic simulations, not an independent benchmark or real-world security evaluation. The AgentDojo integration is limited in scope. Neither repository establishes production-grade security, formal verification, or superiority over other defences. Read the repository threat models and limitations before interpreting results.

### 2. Multimodal Disease Progression Lab

[Repository](https://github.com/sanafirdouse2323-glitch/Multimodal-Disease-Progression-Lab) · [Demo deployment](https://multimodal-disease-progression-lab.onrender.com)

An interactive Streamlit research-methods prototype for comparing models using imaging-related numerical features, wearable-style numerical features, and clinical/visit-level information. It demonstrates next-observed-visit classification, feature-group comparisons, missing-modality stress tests, synthetic causal-effect exercises, and descriptive subgroup evaluation.

**Evidence boundary:** the default workflow uses synthetic data. Its stage codes are generic labels, not a validated medical scale. The application does not accept raw MRI, X-ray, or wearable sensor files, and it is not a diagnostic or prognostic tool. Its documented repeated-seed evaluation found that the tested multimodal models did not exceed the persistence baseline in mean overall accuracy; this negative result is reported rather than presented as a success.

### 3. Diabetes progression regression benchmark

[Repository](https://github.com/sanafirdouse2323-glitch/diabetes-disease-progression-ml)

A comparison of classical regression models and neural-network experiments using the 442-observation diabetes dataset distributed with scikit-learn. The project includes repeated validation, nested model comparison, split-conformal prediction intervals, exploratory subgroup error analysis, and an optional Streamlit demonstration.

**Evidence boundary:** the target is a continuous disease-progression measure, not a diabetes diagnosis. The dataset is small and is not raw hospital data. The documented experiments do not show that neural networks outperform the strongest classical baselines, and the subgroup analysis does not establish fairness.

### 4. Multimodal progression baseline

[Repository](https://github.com/sanafirdouse2323-glitch/multimodal-disease-progression-prototype-2)

A compact PyTorch baseline using synthetic longitudinal cohorts, separate feature-group encoders, multimodal fusion, missingness flags, patient-level splitting, and training-only preprocessing. It is a software and methodology prototype, not clinical evidence.

## Technical toolkit

- **Programming:** Python, C, C++, SQL, Prolog
- **Machine learning and data:** scikit-learn, NumPy, pandas
- **Deep learning:** PyTorch, TensorFlow/Keras
- **Computer vision and image analysis:** OpenCV and image-derived feature workflows
- **NLP:** NLTK, spaCy
- **Visualisation and applications:** Matplotlib, Streamlit
- **Engineering and reproducibility:** Git, Linux, Docker, pytest, GitHub Actions

## Research and engineering principles

- Define the prediction or authorization task precisely before evaluating a system.
- Compare against simple, relevant baselines; do not assume a more complex model is better.
- Separate training, validation, and test data appropriately and guard against leakage.
- Report negative, inconclusive, and positive results.
- Distinguish synthetic experiments, software tests, benchmark results, and real-world evidence.
- Treat security claims as bounded by the threat model, integration assumptions, and tested execution paths.
- Do not describe a prototype as clinically validated, formally verified, independently audited, or production-ready without the corresponding evidence.

## Connect

- [GitHub profile](https://github.com/sanafirdouse2323-glitch)

I welcome thoughtful discussion, research feedback, and collaboration in trustworthy AI, machine learning, multimodal systems, and AI-agent security.
