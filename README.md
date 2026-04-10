# Threat Model Database (TMDB)

Threat modeling is essential for identifying security risks early in the design cycle of modern microelectronic systems. As hardware platforms continue to grow in complexity, they become increasingly exposed to sophisticated and evolving security threats. Despite this growing need, the hardware security community still lacks a comprehensive, standardized, and up-to-date database dedicated to hardware threat models.

The **Threat Model Database (TMDB)** is developed to address this gap. TMDB provides a structured and security-critical database of hardware threat models to support researchers, practitioners, and the broader security community in evaluating vulnerabilities and analyzing potential threats at early design stages.

In our paper "[ATLAS: AI-Assisted Threat-to-Assertion Learning for System-on-Chip Security Verification](https://arxiv.org/abs/2603.01170)" we generated TMDB, which leverages the **National Vulnerability Database (NVD)** as a primary knowledge source. Maintained by the **National Institute of Standards and Technology (NIST)**, NVD is a comprehensive repository of publicly disclosed cybersecurity vulnerabilities spanning software, hardware, and other digital systems. TMDB particularly draws on key NVD components such as:

- **CWE** — Common Weakness Enumeration  
- **CVE** — Common Vulnerabilities and Exposures  
- **CAPEC** — Common Attack Pattern Enumeration and Classification  
- **CWSS** — Common Weakness Scoring System  
- **CVSS** — Common Vulnerability Scoring System  

Using this large corpus of real-world vulnerability data, ATLAS generates threat models for all the existing hardware-related CWEs reported across industry, commercial products, and security practice in NVD database. TMDB not only captures the weaknesses themselves, but also connects them with relevant CVEs and CAPECs to provide a broader view of hardware security threats, real-world examples, and possible countermeasures.

## Why TMDB?

Existing threat modeling tools face several limitations, including incomplete coverage, lack of consistency, and insufficient standardization. One of the most critical gaps is the absence of a universal standard for defining and representing threat models in hardware security.

TMDB addresses this challenge by introducing a **standardized threat model template**. This template defines a common set of elements that should be included in every threat model, enabling consistency, comparability, and reuse across security analyses.

## Standard Threat Model Components

Each threat model in TMDB is organized using the following standardized components:

- **Adversary models** with varying capabilities
- **Assets**
- **Attack surface**
- **Vulnerabilities**
- **Threats**

This structure helps unify threat representation and makes the database suitable for research, benchmarking, security evaluation, and early-stage risk analysis.

## TMDB Generation Process

The figure below illustrates the process of TMDB generation.

![TMDB Generation Process](image.png)

> Replace `image.png` with the filename of your uploaded figure.

## Repository Contents

- `TMDB.xlsx` — The main Threat Model Database file
- `README.md` — Overview of the project, methodology, and repository contents
- `image.png` — Illustration of the TMDB generation workflow

## Potential Use Cases

TMDB can support a variety of research and development activities, including:

- Hardware security threat analysis
- Early-stage threat identification during design
- Security benchmarking and evaluation
- Mapping vulnerabilities to threats and attack patterns
- Supporting automated or AI-assisted threat modeling workflows

## Citation / Acknowledgment

If you use TMDB in your research or project, please cite the relevant paper, project page, or repository-
@misc{tashdid2026atlasaiassistedthreattoassertionlearning,
      title={ATLAS: AI-Assisted Threat-to-Assertion Learning for System-on-Chip Security Verification}, 
      author={Ishraq Tashdid and Kimia Tasnia and Alexander Garcia and Jonathan Valamehr and Sazadur Rahman},
      year={2026},
      eprint={2603.01170},
      archivePrefix={arXiv},
      primaryClass={cs.CR},
      url={https://arxiv.org/abs/2603.01170}, 
}

## Contact

For questions, suggestions, or collaboration opportunities, please open an issue in this repository.
