# Generative AI for Chip Design 

## Table of Contents
- [AutoChip to Generate Functional Verilog](#autochip-to-generate-functional-verilog)
- [VeriThoughts: Enabling Automated Verilog Code Generation using Reasoning and Formal Verification](#verithoughts-enabling-automated-verilog-code-generation-using-reasoning-and-formal-verification)
- [Rome was Not Built in a Single Step: Hierarchical Prompting for LLM-based Chip Design](#rome-was-not-built-in-a-single-step-hierarchical-prompting-for-llm-based-chip-design)
- [Veritas: Deterministic Verilog Code Synthesis from LLM-Generated Conjunctive Normal Form](#veritas-deterministic-verilog-code-synthesis-from-llm-generated-conjunctive-normal-form)
- [PrefixLLM: LLM-aided Prefix Circuit Design](#prefixllm-llm-aided-prefix-circuit-design)
- [LLM-aided Testbench Generation and Bug Detection for Finite-State Machines](#llm-aided-testbench-generation-and-bug-detection-for-finite-state-machines)
- [Hybrid-NL2SVA: LLM-based Natural Language to SystemVerilog Assertion](#hybrid-nl2sva-llm-based-natural-language-to-systemverilog-assertion)
- [Security Assertions by Large Language Models](#security-assertions-by-large-language-models)
- [OpenTitan RAG SVA Generator](#opentitan-rag-sva-generator)
- [LLMPirate: LLMs for Black-box Hardware IP Piracy](#llmpirate-llms-for-black-box-hardware-ip-piracy)
- [C2HLSC: Use LLM to Bridge the Software-to-Hardware Design Gap](#c2hlsc--llms-can-bridge-the-software-to-hardware-design-gap)
- [Masala-CHAI: A Large-Scale SPICE Netlist Dataset for Analog Circuits by Harnessing AI](#masala-chai-a-large-scale-spice-netlist-dataset-for-analog-circuits-by-harnessing-ai)
- [VeriContaminated: Assessing LLM-Driven Verilog Coding for Data Contamination](#vericontaminated-assessing-llm-driven-verilog-coding-for-data-contamination)
- [SALAD: Systematic Assessment of Machine Unlearning on LLM-Aided Hardware Design](#salad-systematic-assessment-of-machine-unlearning-on-llm-aided-hardware-design)
- [Course Project: LLM-Based Verilog Adder Generation and Verification](#course-project-llm-based-verilog-adder-generation-and-verification)
- [Git Submodules (Add / Update / Delete)](#git-submodules-add--update--delete)

---

## AutoChip to Generate Functional Verilog 
**Key Idea:**  
AutoChip generates functional Verilog modules from an initial design prompt and testbench using a selected large language model. Errors from compilation and simulation are fed back into the LLM for repair.

- 📄 **Paper:** https://arxiv.org/abs/2311.04887  
- 💻 **Code:** https://github.com/shailja-thakur/AutoChip.git
- 📑 **Slides:** https://github.com/FCHXWH823/LLM4Hardware/blob/main/slides/ETS%202025%20Tutorial.pptx

---

## VeriThoughts: Automated Verilog Code Generation using Reasoning and Formal Verification
**Key Idea:**  
VeriThoughts is a novel dataset designed for reasoning-based Verilog code generation. We establish a new benchmark framework grounded in formal verification methods to evaluate the quality and correctness of generated hardware descriptions. Additionally, it presents a suite of specialized small-scale models optimized specifically for Verilog generation. Our work addresses the growing need for automated hardware design tools that can produce verifiably correct implementations from high-level specifications, potentially accelerating the hardware development process while maintaining rigorous correctness guarantees.

- 📄 **Paper:** https://arxiv.org/abs/2505.20302  
- 💻 **Code:** https://github.com/wilyub/VeriThoughts

---

## Hierarchical Prompting for LLM-based Hierarchical Verilog Generation
**Key Idea:**  
This tool supports hierarchical Verilog generation for complex hardware modules that standard flat prompting methods cannot achieve. This allows smaller open-source LLMs to compete with large proprietary models. Hierarchical prompting reduces verilig generation time and yields savings on compute costs. This module will detail which LLMs are capable of which applications, and how to apply hierarchical methods in various modes. We will explore case studies of generating complex cores using automatic scripted hierarchical prompts.

- 📄 **Paper:** [https://arxiv.org/abs/2407.18276 ](https://arxiv.org/abs/2407.18276) 
- 💻 **Code:** [https://github.com/ajn313/ROME-LLM/tree/main](https://github.com/ajn313/ROME-LLM/tree/main)
- 📄 **Slides:** [https://github.com/FCHXWH823/LLM4Hardware/blob/main/slides/MLCAD%20ROME%20Presentation.pptx](https://github.com/FCHXWH823/LLM4Hardware/blob/main/slides/MLCAD%20ROME%20Presentation.pptx)

---

## Veritas: Verilog Code Generation from LLM-Generated Conjunctive Normal Form
**Key Idea:**  
Veritas introduces a novel conjunctive normal form (CNF)-guided verilog synthesis methodology. The idea is to have an LLM generate CNF clauses, a format widely used for formal verification and synthesis validation in hardware design. veritas uses it to formally describe the desired circuit functionality. The generated CNF specifications are deterministically converted into Verilog, ensuring correctness by construction.  

- 📄 **Paper:** https://arxiv.org/pdf/2506.00005v1
- 💻 **Code:** [https://github.com/PrithwishBasuRoy/Veritas.git](https://github.com/PrithwishBasuRoy/Veritas.git)
- 📄 **Slides:** [https://github.com/FCHXWH823/LLM4Hardware/blob/main/slides/Veritas-Presentations.pptx](https://github.com/FCHXWH823/LLM4Hardware/blob/main/slides/Veritas-Presentations.pptx)

---

## PrefixLLM: LLM-aided Verilog Generation for Prefix Adder Circuit Design
**Key Idea:**  
Prefix circuits are fundamental components in digital adders, widely used in digital systems due to their efficiency in calculating carry signals. Synthesizing prefix circuits with minimized area and delay is crucial for enhancing the performance of modern computing systems. PrefixLLM transforms the prefix circuit synthesis task into a structured text generation problem, termed the Structured Prefix Circuit Representation (SPCR), and introduces an iterative framework to automatically and accurately generate valid SPCRs. PrefixLLM further presents a design space exploration (DSE) framework that uses LLMs to iteratively search for area- and delay-optimized prefix circuits.

- 📄 **Paper:** https://arxiv.org/abs/2412.02594  
- 💻 **Code:** https://github.com/FCHXWH823/PrefixGPT

---

## LLM-aided Testbench Generation and Bug Detection for Finite-State Machines
**Key Idea:**  
A key aspect of chip design is functional testing, which relies on testbenches to evaluate the functionality and coverage of Verilog designs. This LL-based tool aims to enhance testbench generation by incorporating feedback from commercial-grade Electronic Design Automation tools. Through iterative feedback from these tools, it refines the testbenches to achieve improved test coverage.

- 📄 **Paper:** https://arxiv.org/html/2406.17132v1  
- 🔗 **Code:** https://github.com/jitendra-bhandari/LLM-Aided-Testbench-Generation-for-FSM/

---

## LLM-based Natural Language to SystemVerilog Assertion
**Key Idea:**  
Assertion-based verification is a popular verification technique that involves capturing design intent in a set of assertions that can be used in formal verification or testing-based checking.  However, writing security-centric assertions is a challenging task. This tool helps LLM generate SystemVerilog assertions from natural language input.

- 📄 **Paper:** https://arxiv.org/pdf/2506.21569  
- 💻 **Code:** https://github.com/FCHXWH823/RAG-aided-Assertion-Generation
- 📄 **Slides:** https://github.com/FCHXWH823/LLM4Hardware/blob/main/slides/MLCAD25-Hybrid-NL2SVA.pptx

---

## (Security) Assertions by Large Language Models
**Key Idea:** This tool investigates the use of LLMs for code generation in hardware assertion generation for security, where primarily natural language prompts, such as those one would see as code comments in assertion files, are used to produce SystemVerilog assertions.
- 📄 **Paper:** https://arxiv.org/abs/2306.14027
- 📄 **Slides:** https://github.com/FCHXWH823/LLM4Hardware/blob/main/slides/llm_assertion_slides.pptx

---

## RAG-based SVA Generator for OpenTitan
**Key Idea:** This system combines web scraping, semantic search, and LLMs to generate high-quality SystemVerilog assertions for OpenTitan hardware IP blocks. It downloads documentation from the OpenTitan website, processes it into a searchable knowledge base, and uses AI to generate contextually relevant SVA properties.
- 💻 **Code:** https://github.com/AnandMenon12/OpenTitan_RAG_SVAGEN

---

## LLMPirate: LLMs for Black-box Hardware IP Piracy
**Key Idea:** LLMs are increasingly adopted in hardware design and verification, but their powerful generative capabilities also create new security risks. One unexplored threat vector is intellectual property (IP) piracy: rewriting hardware designs to evade piracy detection tools. LLMPirate that generates pirated circuit design variations capable of consistently bypassing state-of-the-art detection methods. LLMPirate addresses challenges in integrating LLMs with hardware circuit descriptions, scaling to large designs, and ensuring practical efficiency, resulting in an end-to-end automated pipeline.
- 📄 **Paper:** https://arxiv.org/abs/2411.16111
- 📄 **Slides:** https://github.com/FCHXWH823/LLM4Hardware/blob/main/slides/LLMPirate_slides.pptx

---

## C2HLSC:  LLMs can Bridge the Software-to-Hardware Design Gap
**Key Idea:**  
We present a case study using an LLM to rewrite C code for NIST 800-22 randomness tests, a QuickSort algorithm, and AES-128 into HLS-synthesizable C. The LLM iteratively transforms the C code guided by the system prompt and tool's feedback, implementing functions like streaming data and hardware-specific signals. With the hindsight obtained from the case study, we implement a fully automated framework (C2HLSC) to refactor C code into HLS-compatible formats using LLMs. To tackle complex designs, we implement a preprocessing step that breaks down the hierarchy in order to approach the problem in a divide-and-conquer bottom-up way.

- 📄 **Paper:** https://arxiv.org/abs/2412.00214  
- 💻 **Code:** https://github.com/Lucaz97/c2hlsc
- 📄 **Slides:** https://github.com/FCHXWH823/LLM4Hardware/blob/main/slides/C2HLSC%20-%20Neurips%20Tutorial.pptx

---

## Masala-CHAI: A Large-Scale SPICE Netlist Dataset for Analog Circuits by Harnessing AI
**Key Idea:**  
Masala-CHAI is a fully automated framework leveraging large language models (LLMs) to generate Simulation Programs with Integrated Circuit Emphasis (SPICE) netlists. It addresses a long-standing challenge in circuit design automation: automating netlist generation for analog circuits. Automating this workflow could accelerate the creation of fine-tuned LLMs for analog circuit design and verification. In this work, we identify key challenges in automated netlist generation and evaluate multimodal capabilities of state-of-the-art LLMs, particularly GPT-4, in addressing them. 

- 📄 **Paper:** https://arxiv.org/abs/2411.14299  
- 💻 **Code:** https://github.com/jitendra-bhandari/Masala-CHAI

---

## VeriContaminated: Assessing LLM-Driven Verilog Coding for Data Contamination
**Key Idea:**  
We present the first systematic analysis of data contamination in LLM-based Verilog code generation. Using CCD and Min-K% Probability on VerilogEval and RTLLM, we evaluate major models including CodeGen2.5, Mistral 7B, Phi-4 Mini, LLaMA-{1,2,3.1}, GPT-{2,3.5,4o}, DeepSeek-Coder, CodeQwen 1.5, and fine-tuned variants RTLCoder and Verigen. Our results expose significant contamination risks, calling into question current benchmark validity. We further discuss mitigation strategies and quality–fairness trade-offs toward more reliable Verilog LLM evaluation.

- 📄 **Paper:** https://arxiv.org/abs/2503.13572
- 💻 **Code:** https://github.com/DfX-NYUAD/VeriContaminated

---

## SALAD: Systematic Assessment of Machine Unlearning on LLM-Aided Hardware Design
**Key Idea:**  
We present SALAD, the first comprehensive framework for safeguarding LLM-driven hardware design automation. While Large Language Models (LLMs) excel at Verilog code generation, they also introduce data security risks such as benchmark contamination, intellectual property (IP) leakage, and malicious Verilog generation. SALAD employs machine unlearning to selectively remove contaminated datasets, sensitive design artifacts, and harmful code patterns from pre-trained models—without full retraining. Through targeted case studies, we show that unlearning can effectively mitigate security risks while preserving model utility for trustworthy, contamination-free Verilog generation.

- 📄 **Paper:** https://arxiv.org/abs/2506.02089
- 💻 **Code:** https://github.com/DfX-NYUAD/SALAD

---

## Course Project: LLM-Based Verilog Adder Generation and Verification 
**Project Overview** 

This project is designed to explore the capabilities and limitations of Large Language Models (LLMs) in hardware design, specifically in generating and verifying Verilog code for digital adder circuits. The project consists of two interconnected parts that demonstrate the complete workflow from design generation to verification.

**Project Objectives**
- Understand how LLMs can interpret/generate H/W description language (HDL) code
- Practice reverse engineering Verilog designs into natural language specifications
- Evaluate the accuracy of LLM-generated Verilog code against golden reference designs
- Learn to leverage LLMs for automated testbench generation
- Gain hands-on experience with hardware simulation tools (Iverilog)
- Develop critical analysis skills for comparing synthesizable Verilog architectures
  
**Learning Outcomes**
- Ability to analyze and describe digital circuit architectures in natural language
- Understanding of different adder architectures and their trade-offs
- Proficiency in using LLM tools (ChipChat/AutoChip) for hardware design
- Skills in manual code review and verification of HDL designs
- Experience with testbench development and internal signal verification
- Competence in using Iverilog for RTL simulation and debugging

**Project Tutorial:** 
- https://github.com/FCHXWH823/LLM4ChipDesign/blob/main/FinalProjects/Verilog%20Adder%20Generation.pdf 
---

## Git Submodules (Add / Update / Delete)

> This repo uses Git submodules for some components. Use the commands below to add a new submodule, pull updates from its original repo, or remove it.

### Add a submodule
```bash
git submodule add -b <branch_name> <repository_url> <path/to/submodule>
git submodule init
git submodule update
git add .
git commit -m "add <your/module/name>"
git push origin main
```

#### 📌 After adding a new submodule  

Please **also update this README** by adding a new section for the submodule with:  

- **Title** (project name)  
- **Motivation** (short description of its purpose)  
- **Original GitHub repo** (link to the repo)  

This keeps the documentation consistent for future contributors.  

### Update a submodule
```bash
cd <your/module/path>
git fetch
git checkout main
git pull origin main
cd ..
git add <your/module/path>
git commit -m "update <your/module/name>"
git push origin main
```

### Delete a submodule
```bash
git rm <your/module/path>
git commit -m "delete <your/module/name>"
```


