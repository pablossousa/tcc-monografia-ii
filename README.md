# Facial Recognition in CEFET-MG Access Control

![Cover of the work](./Imagens/Capa.png)

This repository contains the final project materials for the undergraduate thesis titled: "Facial Recognition in CEFET-MG Access Control: Technological Modernization Compared to RFID Cards".

The project investigates the feasibility of replacing physical access cards, such as RFID/NFC, with a facial recognition-based authentication system using vector representations of facial features known as embeddings. The proposal combines experimental validation with the development of a functional real-time prototype for authentication in institutional environments.

## About the project

The study was conducted in the context of CEFET-MG and analyzes the possibility of modernizing academic and institutional access control, reducing dependence on physical devices and improving security, practicality, and user experience.

The main objectives of the work include:

- evaluating the technical feasibility of using facial recognition as an alternative to RFID/NFC cards;
- validating the use of facial embeddings and similarity metrics to distinguish identities;
- developing a functional prototype capable of registration, management, and real-time identification;
- considering ethical and privacy aspects in accordance with the LGPD;
- analyzing system robustness using metrics such as FAR and FRR.

## Technologies and approach

The proposed solution uses computer vision and deep learning techniques, with a focus on pretrained models for extracting facial embeddings. The prototype implements:

- face detection and landmark alignment;
- embedding generation using the ArcFace model;
- comparison of face vectors using similarity metrics;
- local storage of biometric data;
- multi-pose enrollment and capture quality assessment;
- temporal voting to improve recognition robustness;
- a graphical interface for user registration and identification.

## Repository structure

- `main.tex` — main LaTeX document;
- `Dados.tex` — project metadata, author, advisor, institution, and pre-textual elements;
- `1-Pre-Textual/` — abstract, summary, and pre-textual sections;
- `2-Textual/` — chapters of the thesis;
- `3-Pos-Textual/` — appendices, annexes, and glossary;
- `Imagens/` — project images, screenshots, and cover artwork;
- `Pacotes/` — package and template configuration files.

## Requirements

To compile the document locally, the following tools are required:

- LaTeX, preferably with `texlive-full` or equivalent;
- `latexmk` for automatic PDF generation;
- a preferred editor such as VS Code with the LaTeX Workshop extension.

## Local execution

Open a terminal in the project folder and run:

```bash
latexmk -pdf -output-directory=out main.tex
```

This command generates the final PDF in a separate output directory, keeping the project root clean.

## Overleaf execution

It is also possible to upload the project to Overleaf and compile it directly in the online environment.

## Author

- Pablo Sousa da Silva

## Supervision

- Advisor: Prof. Me. Diego Ascânio Santos
- Co-advisor: Prof. Dra. Thabatta Moreira Alves de Araújo

## Notes

This repository contains both the academic document of the thesis and the materials required for compiling the monograph, including the text structure, chapters, and visual resources of the project.

---

If you want, I can also create a shorter GitHub-oriented version or a more formal academic version in English.
