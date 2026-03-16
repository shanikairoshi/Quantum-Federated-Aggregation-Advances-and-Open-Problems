# Quantum-Federated-Aggregation-Advances-and-Open-Problems- # Quantum Federated Learning (QFL) Review Repository
Curated repository of recent Quantum Federated Learning (QFL) aggregation strategies with direct links to papers/resources. Includes a comprehensive taxonomy across performance, security, and communication perspectives to support comparison and propose the novel design of more effective aggregation method.

![image](https://github.com/shanikairoshi/Quantum-Federated-Aggregation-Advances-and-Open-Problems/blob/main/Figures/QFLReviewTimeLine_final.png)

This repository organizes key references for a **Quantum Federated Learning (QFL)** review, with emphasis on the three working buckets used in the review:

- **Performance / Efficiency**
- **Security / Privacy**
- **Communication / Networking**

I also keep a separate section for **review/survey papers**, plus a smaller **applications/background** section for domain papers and enabling references that are cited in the broader review.

## How this README is organized

The tables below are aligned with the review logic behind the E–C–P decomposition:

- **E (Encode):** how local information is represented, compressed, filtered, protected, or otherwise prepared before combination.
- **C (Combine):** how the server or network fuses local updates, gradients, kernels, parameters, or messages.
- **P (Postprocess):** how the global model (or client-facing update) is reconstructed, corrected, decoded, broadcast, personalized, or otherwise finalized.

## Link policy

- I prefer **direct paper links** (DOI, arXiv, publisher page, OSTI, IBM blog, etc.).
- Where a stable direct landing page was not easy to verify quickly, I use a **title-search link** so the paper is still one click away.
- A few duplicated items from the raw bibliography are **consolidated** here instead of repeated multiple times.

## Suggested repository structure

```text
.
├── README.md
├── surveys/
├── performance/
├── security/
├── communication/
├── applications/
└── background/
```

---

## Review and survey papers

These are useful as entry points before diving into the method papers.

| Year | Paper | Notes | Access |
|---|---|---|---|
| 2021 | **Federated Quantum Machine Learning** — Chen and Yoo | Foundational early QFL framework. | [DOI](https://doi.org/10.3390/e23040460) |
| 2022 | **Quantum Federated Learning: Remarks and Challenges** — Larasati, Firdaus, and Kim | Early challenge-oriented review. | [Search](https://scholar.google.com/scholar?q=Quantum%20Federated%20Learning%3A%20Remarks%20and%20Challenges) |
| 2022 | **Quantum Federated Learning: Remarks and Challenges** — Larasati, Firdaus, and Kim | Conference version / DOI landing. | [DOI](https://doi.org/10.1109/CSCloud-EdgeCom54946.2022.00014) |
| 2022 | **Quantum federated learning with quantum data** — Chehimi and Saad | Quantum-data setting. | [Search](https://scholar.google.com/scholar?q=Quantum%20federated%20learning%20with%20quantum%20data) |
| 2023 | **Foundations of quantum federated learning over classical and quantum networks** — Chehimi, Chen, Saad, Towsley, and Debbah | Networking-oriented foundations. | [Search](https://scholar.google.com/scholar?q=Foundations%20of%20quantum%20federated%20learning%20over%20classical%20and%20quantum%20networks) |
| 2023 | **Quantum distributed deep learning architectures: Models, discussions, and applications** — Kwak et al. | Distributed quantum learning background. | [Search](https://scholar.google.com/scholar?q=Quantum%20distributed%20deep%20learning%20architectures%3A%20Models%2C%20discussions%2C%20and%20applications) |
| 2024 | **Transitioning from federated learning to quantum federated learning in internet of things: A comprehensive survey** — Qiao et al. | FL→QFL transition survey. | [Search](https://scholar.google.com/scholar?q=Transitioning%20from%20federated%20learning%20to%20quantum%20federated%20learning%20in%20internet%20of%20things%3A%20A%20comprehensive%20survey) |
| 2025 | **Quantum Federated Learning: A Comprehensive Survey** — Nguyen et al. | Large-scale 2025 survey. | [arXiv](https://arxiv.org/abs/2508.15998) |
| 2025 | **Quantum Federated Learning: Architectural Elements and Future Directions** — Sai et al. | Architecture-oriented survey. | [arXiv](https://arxiv.org/abs/2510.17642) |
| 2025 | **Quantum federated learning: a comprehensive literature review of foundations, challenges, and future directions** — Ballester, Cerquides, and Artiles | Open-access review in Quantum Machine Intelligence. | [DOI](https://doi.org/10.1007/s42484-025-00292-2) |
| 2025 | **Towards Heterogeneous Quantum Federated Learning: Challenges and Solutions** — Rahman et al. | Heterogeneity-focused review/discussion. | [arXiv](https://arxiv.org/abs/2511.22148) |
| 2025 | **When Federated Learning Meets Quantum Computing: Survey and Research Opportunities** — Mathur, Gupta, and Das | Broad hybrid FL+QC survey. | [arXiv](https://arxiv.org/abs/2504.08814) |
| 2026 | **Exploring quantum federated learning: Algorithms, applications, and challenges** — Innan et al. | Book chapter review. | [DOI](https://doi.org/10.1016/B978-0-44-330259-6.00010-4) |
| 2026 | **Quantum-Federated Learning: A review of frameworks and applications for Sustainable Development Goals (SDGs)** — Kumar and Verma | Sustainability-oriented review. | [Search](https://scholar.google.com/scholar?q=Quantum-Federated%20Learning%3A%20A%20review%20of%20frameworks%20and%20applications%20for%20Sustainable%20Development%20Goals) |


## Performance / Efficiency

| Year | Paper | Notes | Access |
|---|---|---|---|
| 2021 | **QuantumFed: A Federated Learning Framework for Collaborative Quantum Training** — Xia and Li | QuanFed / vanilla QFL baseline. | [arXiv](https://arxiv.org/abs/2106.09109) |
| 2022 | **Quantum federated learning with decentralized data** — Huang, Tan, and Xu | qSGD-style decentralized QFL. | [Search](https://scholar.google.com/scholar?q=Quantum%20federated%20learning%20with%20decentralized%20data) |
| 2023 | **Optimizing Quantum Federated Learning Based on Federated Quantum Natural Gradient Descent** — Qi, Zhang, and Tejedor | FQNGD / natural-gradient aggregation. | [arXiv](https://arxiv.org/abs/2303.08116) |
| 2024 | **A personalized quantum federated learning** — Gurung and Pokhrel | Personalized QFL. | [Search](https://scholar.google.com/scholar?q=A%20personalized%20quantum%20federated%20learning) |
| 2024 | **A quantum federated learning framework for classical clients** — Song et al. | CC-QFL / classical-client-compatible QFL. | [DOI](https://doi.org/10.1007/s11433-023-2337-2) |
| 2024 | **Distributed quantum machine learning: Federated and model-parallel approaches** — Wu, Hu, and Li | Federated/model-parallel DQML overview. | [Search](https://scholar.google.com/scholar?q=Distributed%20quantum%20machine%20learning%3A%20Federated%20and%20model-parallel%20approaches) |
| 2024 | **FedQNN: Federated Learning using Quantum Neural Networks** — Innan et al. | Hybrid QNN-based QFL. | [arXiv](https://arxiv.org/abs/2403.10861) |
| 2024 | **QFSM: A Novel Quantum Federated Learning Algorithm for Speech Emotion Recognition With Minimal Gated Unit in 5G IoV** — Qu et al. | Sequence model / QMGU-based QFL. | [DOI](https://doi.org/10.1109/TIV.2024.3370398) |
| 2024 | **Quantum Federated Learning Experiments in the Cloud with Data Encoding** — Pokhrel et al. | Data-encoding and adaptive cloud QFL. | [arXiv](https://arxiv.org/abs/2405.00909) |
| 2024 | **Toward Uniform Quantum Federated Aggregation: Heterogeneity Exclusion Using Entropy and Fidelity** — Son and Park | Entropy/fidelity-based client exclusion. | [DOI](https://doi.org/10.1109/JIOT.2024.3488180) |
| 2024 | **Towards Federated Learning on the Quantum Internet** — Sünkel et al. | Topology and routing-aware distributed QML/QFL. | [Search](https://scholar.google.com/scholar?q=Towards%20Federated%20Learning%20on%20the%20Quantum%20Internet) |
| 2025 | **Enhancing Quantum Federated Learning with Fisher Information-Based Optimization** — Bhatia and Kais | QFedFisher / Fisher-guided update weighting. | [Search](https://scholar.google.com/scholar?q=Enhancing%20Quantum%20Federated%20Learning%20with%20Fisher%20Information-Based%20Optimization) |
| 2025 | **Federated Quantum Kernel-Based Long Short-term Memory for Human Activity Recognition** — Hsu et al. | Fed-QK-LSTM / kernel-gated HAR. | [arXiv](https://arxiv.org/abs/2508.06078) |
| 2025 | **Layerwise Federated Learning for Heterogeneous Quantum Clients using Quorus** — Han et al. | Heterogeneous-depth clients / layerwise loss. | [arXiv](https://arxiv.org/abs/2510.06228) |
| 2025 | **Quantum federated learning with pole-angle quantum local training and trainable measurement** — Park et al. | Pole-angle local training / selective sharing. | [Search](https://scholar.google.com/scholar?q=Quantum%20federated%20learning%20with%20pole-angle%20quantum%20local%20training%20and%20trainable%20measurement) |


## Security / Privacy

| Year | Paper | Notes | Access |
|---|---|---|---|
| 2021 | **OQFL: An optimized quantum-based federated learning framework for defending against adversarial attacks in intelligent transportation systems** — Yamany, Moustafa, and Turnbull | Adversarially robust QFL-inspired ITS application. | [Search](https://scholar.google.com/scholar?q=OQFL%20An%20optimized%20quantum-based%20federated%20learning%20framework%20for%20defending%20against%20adversarial%20attacks%20in%20intelligent%20transportation%20systems) |
| 2021 | **Quantum federated learning through blind quantum computing** — Li, Lu, and Deng | BQC-style delegated privacy. | [Search](https://scholar.google.com/scholar?q=Quantum%20federated%20learning%20through%20blind%20quantum%20computing) |
| 2022 | **Federated Learning with Quantum Secure Aggregation** — Zhang et al. | Quantum secure aggregation via entanglement/phase encoding. | [arXiv](https://arxiv.org/abs/2207.07444) |
| 2022 | **Privacy-preserving intelligent resource allocation for federated edge learning in quantum internet** — Xu et al. | Quantum-internet secure/resource layer; adjacent reference. | [Search](https://scholar.google.com/scholar?q=Privacy-preserving%20intelligent%20resource%20allocation%20for%20federated%20edge%20learning%20in%20quantum%20internet) |
| 2023 | **CryptoQFL: quantum federated learning on encrypted data** — Chu, Jiang, and Chen | Encrypted-data QFL. | [Search](https://scholar.google.com/scholar?q=CryptoQFL%20quantum%20federated%20learning%20on%20encrypted%20data) |
| 2023 | **HQK-FL: Hybrid-Quantum-Key-Based Secure Federated Learning for Distributed Multi-Center Clinical Studies** — Park and Lee | Hybrid quantum keys for secure FL. | [DOI](https://doi.org/10.22967/HCIS.2023.13.045) |
| 2023 | **Multi-client distributed blind quantum computation with the Qline architecture** — Polacchi et al. | Relevant multi-client blind-QC building block. | [Search](https://scholar.google.com/scholar?q=Multi-client%20distributed%20blind%20quantum%20computation%20with%20the%20Qline%20architecture) |
| 2023 | **Secure communication model for quantum federated learning: A post quantum cryptography (PQC) framework** — Gurung, Pokhrel, and Li | PQC framework for QFL messaging. | [arXiv](https://arxiv.org/abs/2304.13413) |
| 2023 | **Secure communication model for quantum federated learning: A proof of concept** — Gurung, Pokhrel, and Li | Proof-of-concept secure QFL communication. | [Search](https://scholar.google.com/scholar?q=Secure%20communication%20model%20for%20quantum%20federated%20learning%3A%20A%20proof%20of%20concept) |
| 2023 | **Unsupervised Federated Quantum GAN for Optimizing Wireless Communications** — Jamaluddin, Narottama, and Shin | Unsupervised FQGAN / privacy-preserving wireless setting. | [Search](https://scholar.google.com/scholar?q=Unsupervised%20Federated%20Quantum%20GAN%20for%20Optimizing%20Wireless%20Communications) |
| 2024 | **ESQFL: Digital twin-driven explainable and secured quantum federated learning for voltage stability assessment in smart grids** — Ren et al. | Explainability + security + smart-grid setting. | [Search](https://scholar.google.com/scholar?q=ESQFL%20Digital%20twin-driven%20explainable%20and%20secured%20quantum%20federated%20learning%20for%20voltage%20stability%20assessment%20in%20smart%20grids) |
| 2024 | **Enhancing quantum security over federated learning via post-quantum cryptography** — Li, Chen, and Liu | PQC signatures for FL; useful for secure QFL stacks. | [arXiv](https://arxiv.org/abs/2409.04637) |
| 2024 | **Federated learning with quantum computing and fully homomorphic encryption: A novel computing paradigm shift in privacy-preserving ML** — Dutta et al. | QFed+FHE concept paper. | [arXiv](https://arxiv.org/abs/2409.11430) |
| 2024 | **Federated quantum machine learning with differential privacy** — Rofougaran, Yoo, and Tseng | DP guarantees in FQML/QFL. | [Search](https://scholar.google.com/scholar?q=Federated%20quantum%20machine%20learning%20with%20differential%20privacy) |
| 2024 | **MQFL-FHE: Multimodal quantum federated learning framework with fully homomorphic encryption** — Dutta et al. | Multimodal/FHE-protected QFL. | [arXiv](https://arxiv.org/abs/2412.01858) |
| 2024 | **Quantum fuzzy federated learning for privacy protection in intelligent information processing** — Qu, Zhang, and Tiwari | Privacy-preserving fuzzy/QFL variant. | [Search](https://scholar.google.com/scholar?q=Quantum%20fuzzy%20federated%20learning%20for%20privacy%20protection%20in%20intelligent%20information%20processing) |
| 2024 | **Toward uniform quantum federated aggregation: Heterogeneity exclusion using entropy and fidelity** — Son and Park | Often also read as a secure/robust client-filtering mechanism. | [DOI](https://doi.org/10.1109/JIOT.2024.3488180) |
| 2025 | **Differentially Private Federated Quantum Learning via Quantum Noise** — Pokharel et al. | DP-QFL via injected quantum noise. | [arXiv](https://arxiv.org/abs/2508.20310) |
| 2025 | **Federated Quantum Kernel Learning for Anomaly Detection in Multivariate IoT Time-Series** — Chen et al. | Kernel-based anomaly-detection QFL. | [arXiv](https://arxiv.org/abs/2511.02301) |
| 2025 | **Practical quantum federated learning and its experimental demonstration** — Liu et al. | Distributed quantum secret keys + experimental demo. | [arXiv](https://arxiv.org/abs/2501.12709) |
| 2025 | **QFAL: Quantum federated adversarial learning** — El Maouaki et al. | Adversarial robustness in QFL. | [arXiv](https://arxiv.org/abs/2502.21171) |
| 2025 | **Quantum delegated and federated learning via quantum homomorphic encryption** — Li and Deng | Delegated QHE/QOTP-flavored secure learning. | [arXiv](https://arxiv.org/abs/2409.19359) |
| 2025 | **Quantum federated learning through ancilla-driven quantum computation** — Shi et al. | Ancilla-driven private/delegated execution. | [Search](https://scholar.google.com/scholar?q=Quantum%20federated%20learning%20through%20ancilla-driven%20quantum%20computation) |
| 2025 | **Quantum-enhanced blockchain federated learning via quantum Byzantine agreement** — Liu et al. | QBA-style robust and verified aggregation. | [Search](https://scholar.google.com/scholar?q=Quantum-enhanced%20blockchain%20federated%20learning%20via%20quantum%20Byzantine%20agreement) |
| 2026 | **A novel blockchain-federated learning framework with quantum neural networks and wavelet transforms for secure IoT healthcare monitoring** — Reddy et al. | Blockchain + QNN healthcare monitoring. | [Search](https://scholar.google.com/scholar?q=A%20novel%20blockchain-federated%20learning%20framework%20with%20quantum%20neural%20networks%20and%20wavelet%20transforms%20for%20secure%20IoT%20healthcare%20monitoring) |


## Communication / Networking

| Year | Paper | Notes | Access |
|---|---|---|---|
| 2022 | **Quantum Federated Learning for Wireless Communications** — Pujahari and Tanwar | Book-chapter style communication-oriented background. | [Search](https://scholar.google.com/scholar?q=Quantum%20federated%20learning%20for%20wireless%20communications) |
| 2022 | **Quantum Federated Learning with Entanglement Controlled Circuits and Superposition Coding** — Yun et al. | eSQFL / superposition coding. | [arXiv](https://arxiv.org/abs/2212.01732) |
| 2022 | **Slimmable Quantum Federated Learning** — Yun et al. | Split upload / dynamic-width sharing. | [arXiv](https://arxiv.org/abs/2207.10221) |
| 2023 | **Decentralized Quantum Federated Learning for Metaverse: Analysis, Design and Implementation** — Gurung, Pokhrel, and Li | Decentralized/metaverse-oriented QFL. | [arXiv](https://arxiv.org/abs/2306.11297) |
| 2023 | **Federated Quantum Neural Network With Quantum Teleportation for Resource Optimization in Future Wireless Communication** — Narottama and Shin | Teleportation-assisted fusion / wireless resource optimization. | [Search](https://scholar.google.com/scholar?q=Federated%20Quantum%20Neural%20Network%20With%20Quantum%20Teleportation%20for%20Resource%20Optimization%20in%20Future%20Wireless%20Communication) |
| 2023 | **Non-IID quantum federated learning with one-shot communication complexity** — Zhao | One-shot / inference-lean communication. | [Search](https://scholar.google.com/scholar?q=Non-IID%20quantum%20federated%20learning%20with%20one-shot%20communication%20complexity) |
| 2023 | **Quantum-empowered federated learning in space-air-ground integrated networks** — Wang et al. | Quantum-enabled network scheduling / communication backdrop. | [Search](https://scholar.google.com/scholar?q=Quantum-empowered%20federated%20learning%20in%20space-air-ground%20integrated%20networks) |
| 2024 | **Dynamic quantum federated learning for satellite-ground integrated systems using slimmable quantum neural networks** — Park, Jung, and Kim | Satellite-ground communication-aware QFL. | [DOI](https://doi.org/10.1109/ACCESS.2024.3392429) |
| 2024 | **NAC-QFL: Noise Aware Clustered Quantum Federated Learning** — Sahu and Gupta | Noise-aware clustering and circuit partitioning. | [arXiv](https://arxiv.org/abs/2406.14236) |
| 2024 | **Quantum Federated Learning with Quantum Networks** — Wang, Tseng, and Yoo | Quantum-network transport / ICASSP 2024. | [OSTI PDF](https://www.osti.gov/servlets/purl/2549222) |
| 2024 | **Variational quantum circuit and quantum key distribution-based quantum federated learning: A case of smart grid dynamic security assessment** — Ren et al. | QKD-enabled smart-grid QFL. | [Search](https://scholar.google.com/scholar?q=Variational%20quantum%20circuit%20and%20quantum%20key%20distribution-based%20quantum%20federated%20learning%3A%20A%20case%20of%20smart%20grid%20dynamic%20security%20assessment) |
| 2025 | **Chained continuous quantum federated learning framework** — Gurung and Pokhrel | Serverless chained relay / continuous QFL. | [Search](https://scholar.google.com/scholar?q=Chained%20continuous%20quantum%20federated%20learning%20framework) |
| 2025 | **Communication Efficient Adaptive Model-Driven Quantum Federated Learning** — Gurung and Pokhrel | Adaptive/model-driven communication-efficient QFL. | [arXiv](https://arxiv.org/abs/2506.04548) |
| 2026 | **QFI-Opt: Communication-Efficient Quantum Federated Learning via Quantum Fisher Information** — Zhang et al. | Pruning / Fisher-information communication efficiency. | [Search](https://scholar.google.com/scholar?q=QFI-Opt%20Communication-Efficient%20Quantum%20Federated%20Learning%20via%20Quantum%20Fisher%20Information) |


## Applications / Domains

| Year | Paper | Notes | Access |
|---|---|---|---|
| 2023 | **Toward Quantum Federated Learning** — Ren et al. | Earlier arXiv version of the Ren et al. line. | [arXiv](https://arxiv.org/abs/2306.09912) |
| 2024 | **Quantum computing in the next-generation computational biology landscape: from protein folding to molecular dynamics** — Pal et al. | Computational biology backdrop. | [Search](https://scholar.google.com/scholar?q=Quantum%20computing%20in%20the%20next-generation%20computational%20biology%20landscape%3A%20from%20protein%20folding%20to%20molecular%20dynamics) |
| 2024 | **mRNA secondary structure prediction using utility-scale quantum computers** — Alevras et al. | Quantum application motivation. | [Search](https://scholar.google.com/scholar?q=mRNA%20secondary%20structure%20prediction%20using%20utility-scale%20quantum%20computers) |
| 2025 | **Case study: Moderna and IBM use quantum computing to model mRNA structure** — Cherry | Industry blog / application context. | [IBM](https://www.ibm.com/quantum/blog/moderna-case-study) |
| 2025 | **Generating three-dimensional genome structures with a variational quantum algorithm** — Siciliano and Wang | Quantum genomics application. | [Search](https://scholar.google.com/scholar?q=Generating%20three-dimensional%20genome%20structures%20with%20a%20variational%20quantum%20algorithm) |
| 2025 | **Quantum algorithm for identifying RNA 3D motifs by processing RNA secondary structure graphs** — Fang et al. | RNA structural analysis. | [Search](https://scholar.google.com/scholar?q=Quantum%20algorithm%20for%20identifying%20RNA%203D%20motifs%20by%20processing%20RNA%20secondary%20structure%20graphs) |
| 2025 | **Toward Quantum Federated Learning** — Ren et al. | Broad application-oriented TNNLS article. | [Search](https://scholar.google.com/scholar?q=Toward%20Quantum%20Federated%20Learning) |
| 2025 | **Towards secondary structure prediction of longer mRNA sequences using a quantum-centric optimization scheme** — Kumar et al. | Quantum bioinformatics application. | [arXiv](https://arxiv.org/abs/2505.05782) |
| 2026 | **FedVQC for Genomic Data: A Quantum-Enhanced Privacy Approach** — Gawande, Hire, and Dhande | Genomic QFL application. | [Search](https://scholar.google.com/scholar?q=FedVQC%20for%20Genomic%20Data%3A%20A%20Quantum-Enhanced%20Privacy%20Approach) |
| 2026 | **QFedPhish: A Quantum-Inspired Federated Learning Approach for Detecting AI-Generated Phishing Attacks** — Malik and Qaisar | Cybersecurity application. | [Search](https://scholar.google.com/scholar?q=QFedPhish%3A%20A%20Quantum-Inspired%20Federated%20Learning%20Approach%20for%20Detecting%20AI-Generated%20Phishing%20Attacks) |
| 2026 | **Quantum-Enhanced Federated Learning Architecture for Privacy-Preserving Smart Grid IoT Security** — Baazeem | Smart-grid / IoT application. | [Search](https://scholar.google.com/scholar?q=Quantum-Enhanced%20Federated%20Learning%20Architecture%20for%20Privacy-Preserving%20Smart%20Grid%20IoT%20Security) |


## Background / Foundations

| Year | Paper | Notes | Access |
|---|---|---|---|
| 1994 | **Algorithms for quantum computation: discrete logarithms and factoring** — Shor | Shor’s algorithm. | [Search](https://scholar.google.com/scholar?q=Algorithms%20for%20quantum%20computation%20discrete%20logarithms%20and%20factoring) |
| 1996 | **A fast quantum mechanical algorithm for database search** — Grover | Grover’s algorithm. | [Search](https://scholar.google.com/scholar?q=A%20fast%20quantum%20mechanical%20algorithm%20for%20database%20search) |
| 2009 | **Universal blind quantum computation** — Broadbent, Fitzsimons, and Kashefi | Blind quantum computation foundation. | [Search](https://scholar.google.com/scholar?q=Universal%20blind%20quantum%20computation) |
| 2010 | **Quantum computation and quantum information** — Nielsen and Chuang | Standard QC textbook. | [Search](https://scholar.google.com/scholar?q=Quantum%20computation%20and%20quantum%20information%20Nielsen%20Chuang) |
| 2018 | **PennyLane: Automatic differentiation of hybrid quantum-classical computations** — Bergholm et al. | Hybrid QML tooling. | [arXiv](https://arxiv.org/abs/1811.04968) |
| 2019 | **Quantum chemistry in the age of quantum computing** — Cao et al. | Broader QC application landscape. | [Search](https://scholar.google.com/scholar?q=Quantum%20chemistry%20in%20the%20age%20of%20quantum%20computing) |
| 2020 | **TensorFlow Quantum: A software framework for quantum machine learning** — Broughton et al. | QML tooling. | [arXiv](https://arxiv.org/abs/2003.02989) |
| 2020 | **Verifying results of the IBM Qiskit quantum circuit compilation flow** — Burgholzer, Raymond, and Wille | Compiler/toolchain reliability. | [Search](https://scholar.google.com/scholar?q=Verifying%20results%20of%20the%20IBM%20Qiskit%20quantum%20circuit%20compilation%20flow) |
| 2022 | **Introduction to classical and quantum computing** — Wong | Introductory background text. | [Search](https://scholar.google.com/scholar?q=Introduction%20to%20classical%20and%20quantum%20computing%20Thomas%20G%20Wong) |
| 2024 | **The future of two-dimensional semiconductors beyond Moore’s law** — Kim et al. | Hardware-context reference. | [Search](https://scholar.google.com/scholar?q=The%20future%20of%20two-dimensional%20semiconductors%20beyond%20Moore%27s%20law) |


---

## Mapping to the review tables

The two LaTeX tables in the manuscript can be mirrored in the repository as follows:

- **Performance / Efficiency:** QuanFed, qSGD-style QFL, FQNGD, QFEA, FedQNN, QFSM, Quorus, CDE/EFE, CC-QFL, personalized QFL, MCMDQFL, DQML, QFedFisher, Fed-QK-LSTM, PoleQSNN.
- **Security / Privacy:** QBA, QSA, practical QFL with distributed secret keys, QFAL, blind-QC QFL, CryptoQFL, OQFL, ESQFL, ADQCQFL, QFL-DP, PQCQFL, QFed+FHE, MQFL-FHE, delegated QHE/QOTP, Qline-style blind multi-client computation, HQK-FL, QFFL, UFQGAN, DP-QFL, FQKL, BC-QFL.
- **Communication / Networking:** NAC-QFL, chained/continuous QFL, model-driven QFL, quantum-network QFL, one-shot/non-IID communication, teleportation-assisted QFL, SlimQFL, eSQFL, pole-angle selective upload, satellite-ground QFL, QKD-assisted smart-grid QFL, QFI-Opt.

---

## Notes for maintainers

1. For a paper-centric repository, create one Markdown note per paper inside the matching folder.
2. Use a consistent filename style, e.g. `2025_quorus.md` or `2024_fedqnn.md`.
3. In each paper note, record:
   - problem setting,
   - quantum/classical split,
   - aggregation rule,
   - security mechanism,
   - communication assumption,
   - datasets / applications,
   - key limitation,
   - relationship to your own aggregation framework.
4. For duplicates in the original bibliography, keep **one canonical entry** in the repo and mention alternative versions inside that note.

---

## Minimal template for each paper note

```markdown
# Paper title

- **Authors:** 
- **Year:** 
- **Venue:** 
- **Link:** 

## Why it matters
...

## E–C–P signature
- **E:** 
- **C:** 
- **P:** 

## Main novelty
...

## Strengths
...

## Limitations
...

## Relation to A2G / aggregation-centric QFL review
...
```

---

## Citation hygiene

Before finalizing the repository, it is worth normalizing:
- duplicate entries,
- inconsistent capitalization (e.g., `Quantum federated learning` vs `Quantum Federated Learning`),
- venue inconsistencies (`arXiv preprint`, conference paper, journal version),
- and title variants that refer to the same line of work.

Next possible extensions:
1. a **GitHub-ready polished final version with badges and internal anchors**;
2. a **full paper-by-paper Markdown note set** for the `performance/`, `security/`, and `communication/` folders.
