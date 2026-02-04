---
layout: default
title: Tasks
---

# Tasks

---

[Home](./) | [Call for papers](./CFP) | [Important dates](./dates) | [Tasks](./tasks)  | [Tools](./tools) | 
[Program](./program) | [Publications](./publications) | [Organizers](./organizers) | [Contact](./contact) | [CLEF-2025](https://simpletext-project.com/2025/)

---

## How to participate
In order to participate, you should sign up at the [CLEF](https://clef2025.clef-initiative.eu/index.php?page=Pages/registration.html) website: [https://clef2025-labs-registration.dei.unipd.it/](https://clef2025-labs-registration.dei.unipd.it/). 

All team members should join the SimpleText mailing list:
[https://groups.google.com/g/simpletext](https://groups.google.com/g/simpletext). 

The data will be made available to all registered participants.

## Task 1: Text Simplification: Simplify scientific text
The CLEF 2026 SimpleText track introduced the Cochrane-auto corpus, derived from biomedical literature abstracts and lay summaries from Cochrane systematic reviews. This corpus represents a significant expansion into the biomedical domain, building on methodologies used for datasets like Wiki-auto and Newsela-auto.

Cochrane-auto provides authentic parallel data produced by the same authors, enabling true document-level simplification. It incorporates advanced simplification techniques such as sentence merging, reordering, and alignment with discourse structure. This approach contrasts with more standard simplification corpora by realigning data at the paragraph, sentence, and document levels.

From that we extract two subtasks:

### Task 1.1 - Sentence-level Scientific Text Simplification
The goal of this task is to simplify whole sentences extracted from the Cochrane-auto dataset

### Task 1.2 - Document-level Scientific Text Simplification 
The goal of this task is to simplify whole documents extracted from the Cochrane-auto dataset

### Evaluation
To evaluate results we will use standard automatic evaluation measures (SARI, BLEU, LENS, BERTscore, etc.) in combination with human assessment of samples of the submissions by translation students and professionals.

## Task 2: Controlled Creativity: Identify and Avoid Hallucination

Task 2 focuses on identifying and evaluating creative generation and information distortion in text simplification.

### Task 2.1 - Identify Creative Generation at Document Level

This task aims to detect creative generation at the abstract or document level. Participants will analyze system outputs from previous years, along with deliberately generated outputs from known models. The goal is to identify which sentences are fully grounded in the source text, both without access to the original sentences and with access to them. Additionally, sentences that introduce significant new content must be labeled. This task serves as a post-hoc identification or explanation challenge.

### Task 2.2 - Detect and Classify Information Distortion Errors in Simplified Sentences

This task focuses on detecting information distortion in simplified sentences and classifying the types of errors.

### Task 2.3 - Avoid Creative Generation and Perform Grounded Generation by Design

This task introduces a text alignment challenge, emphasizing grounded generation over creative generation. This task mirrors Task 1 on text simplification and requires submissions in paired runs, both with and without explicit source attribution.

### Evaluation
 - Task 2.1 is essentially a sentence label task, evaluated in the standard way (Precision, Recall, F1). For token-level evaluation, we use standard Jaccard.
 - Task 2.2 is evaluated using standard automatic classification measures. 
 - Task 2.3 will be evaluated by both standard automatic measures and human evaluation, similar to Task 1 on Text Simplification above. The paired runs enable us to sample  differences at the sentence and phrase levels and evaluate them efficiently, using tools like MT Unbabel.

## Task 3: LeaderBoardQA

Task 3, known as LeaderBoardQA, extends a pilot task from CLEF 2024 focused on information extraction in scientific documents. Participants are tasked with constructing a leaderboard-like output by using domain-specific question-answering (QA) to retrieve performance metrics on AI models. This task challenges participants to gather exact performance data and relevant metrics on specified AI models, or on models and benchmarks combined, directly from a scientific corpus. The approach encourages using advanced Large Language Models (LLMs) and Retrieval-Augmented Generation (RAG) systems, with both open-corpus and closed-book submission formats supported.

### Description

LeaderBoardQA requires extracting specific ânuggetsâ of information related to AI model performance from a full-text scientific corpus. These nuggets include exact details on model performance and relevant metrics, assessed across a range of benchmarks. Participants are expected to leverage LLMs and RAGs for accurate and reliable extraction, aiding in the construction of a comprehensive leaderboard for model performance. Building upon CLEF 2024's SimpleText SOTA task, this extension broadens its scope to evaluate the potential of domain-specific QA in generating benchmark datasets and improving AI performance transparency.

### Data and evaluation

For LeaderBoardQA, CLEF will reuse community-aligned training data from CLEF 2024 and enhance it with human-annotated gold standards to support rigorous evaluation. The task will follow QA evaluation protocols tailored for LLM and RAG systems, with results analysed against a comprehensive gold-standard corpus. This dataset will serve as a critical resource for benchmarking QA performance on scientific information extraction tasks, as detailed in the CLEF 2024 SimpleText Task 4 overview paper.

## Task 4: SimpleText 2024 Revisited

CLEF 2025 introduces a restructured SimpleText track, aimed at adapting to new objectives and participant interests. Task 4 serves as a transitional track, potentially continuing work from CLEF 2024 tasks based on demand. Specifically, it considers re-running Task 1 on Content Selection (abstract retrieval) and Task 2 on Complexity Spotting (identifying and explaining difficult concepts). The continuation of these tracks is contingent on active interest and input from participants and organisers, with discussions planned at the CLEF 2024 conference in Grenoble.

### Description

CLEF 2025 SimpleText is very different from the earlier years. In order to facilitate the transition to the new track setup, we consider continuing one of the other CLEF 2024 SimpleText tracks (Task 1 on Content Selection: abstract re- trieval, Task 2 on Complexity Spotting: identifying and explaining difficult concepts). We will only continue those activities at the request of, and with sufficient interest from, our active participants. We will discuss this with participants and the current team of organisers at CLEF 2024 in Grenoble

### Data and evaluation

For further reference on methodology and evaluation criteria, details are available in the LNCS track overview paper by Ermakova et al. (2024b), as well as in the CEUR task overview papers for CLEF 2024 SimpleText Task 1 (Sanjuan et al., 2024) and Task 2 (Di Nunzio et al., 2024).