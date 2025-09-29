# ai-agile-framework
Human-Centered AI-Enabled Transformation of User Stories into Architectural Blueprints in Large-Scale Agile Development
This repository contains the prototype implementation of the AI-enabled, semi-automated framework introduced in the research paper “Human-Centered AI-Enabled Transformation of User Stories into Architectural Blueprints in Large-Scale Agile Development.”

#Overview

The framework addresses a long-standing challenge in large-scale agile software development: the disconnect between informal user stories and formal architectural models. It provides an end-to-end pipeline that:

Preprocesses and evaluates user story quality.

Applies semantic clustering and topic modeling.

Maps story clusters to architectural components.

Generates UML-based architectural blueprints for sprint-level planning.

The design emphasizes:

Human-centeredness (keeping user intent visible in architecture).

Traceability (preserving links between requirements and design).

Scalability (capable of handling enterprise backlogs).

Extensibility (modules can be swapped or fine-tuned).

Features

NLP Preprocessing: Tokenization, lemmatization, stopword removal.

Quality Assessment: Integration with AQUSA/StoryLine for user story validation.

Semantic Analysis: Dual approach using TF-IDF + LDA and BERT embeddings + K-Means.

Architectural Mapping: Hybrid rule-based and supervised classification for component assignment.

Artifact Generation: Automated creation of UML component and use case diagrams.

Repository Contents

preprocessing.py → NLP preprocessing pipeline

quality_assessment.py → User story quality analysis

semantic_clustering.py → TF-IDF, LDA, and BERT-based clustering

architectural_mapping.py → Mapping clusters to architectural components

uml_generator.py → UML artifact generation (PlantUML integration)

example_dataset.csv → Sample user stories dataset (anonymized)
