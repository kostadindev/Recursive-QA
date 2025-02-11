
# Recursive QA: An NLP Annotation Framework

Recursive QA is an NLP annotation framework that replaces traditional labeling methods with a question-answering approach. By leveraging the constituency parse tree of a sentence, it guides annotators through selecting from generated question-answer pairs, streamlining the annotation process and improving quality control.

![image](https://github.com/user-attachments/assets/d285775c-c626-4655-8768-bfc3bc83f2e3)

## Features

- **Question-Answer Based Annotation:** Simplifies manual span and relation labeling by using QA pairs.
- **Constituency Parse Tree Integration:** Utilizes the syntactic structure of sentences to guide annotations.
- **Visualizations:** Offers clear and interactive visual representations to enhance annotation clarity.
- **User Management:** Supports account creation, role management, and user-specific tracking.
- **History Tracking:** Maintains logs of annotation history for review and quality assurance.

## Inspiration

This project was developed as part of my senior honors thesis, **Recursive QA**, under the guidance of **Professor Niranjan Balasubramanian**. Inspired by human-AI collaboration in previous projects, I aimed to simplify traditional NLP annotation processes through an intuitive QA-based approach.

## How It Works

1. **Parse Tree Analysis:** The system analyzes the constituency parse tree of a given sentence.
2. **QA Pair Generation:** Based on the syntactic structure, it generates relevant question-answer pairs.
3. **Guided Annotation:** Annotators are guided top-down through the tree, selecting appropriate QA pairs.
4. **Span and Relation Resolution:** Leaf-level answers are identified as spans, while QA links define relations.

## Evaluation

The framework was tested on **SpecNFS**, a dataset designed for extracting formal models from Network File System (NFS) specifications (RFCs). Key results include:

- **Annotation Speed:** Average of 25 seconds per sentence.
- **Annotator Agreement:** Approximately 80% agreement rate between annotators, a high figure given the complexity of the text and representation language.

## Tech Stack

- **React:** Frontend framework for building an intuitive and interactive user interface.
- **Flask:** Backend API to handle annotation logic, QA pair generation, and server-side processing.
- **MongoDB:** NoSQL database for storing user data, annotation history, and project information.
