# Multilingual Natural Language Processing - *2020 Spring*
##### Yulia Tsvetkov, Graham Neubig and Alan Black
##### *Lnaugage Technologies Institie, Carnegie Mellon University*

## Lecture 1. Linguistics, multilinguality, and Multilingual Training

### Yulia
1. Tokenization + Disambiguation
2. Morphosyntactic analysis
3. Morphological Processing
4. Syntactic parsing
5. Semantic analysis

### Graham
1. Sequence Labeling / Classification
2. Machine Translation and Sequence-to-Sequence Models
3. Syntax - Syntactic formalisms and Syntactic typology (difference language different position)
4. Active Learning

### Alan
1. Speech
2. Grammar
3. Phonology
4. Hindi

## Lecture 2. Typology: The Space of Languages

### Introduction
#### Linguistic diversity
languages based on English

#### Low resource Languages
1. 460 languages in India
2. lans in Africa

### Approaches to low-resource/multilingual NLP
Manual curation or annotation is expensive

**Approach**:
1. *Unsupervised learning*
2. *Cross-lingual transfer learning*
  * Transfer of annotations (using alignments or other cross-lingual bridges)
  * Transfer of models - train a model in a resource-rich language and transfer is to the corresponding resource-poor language
3. *Zero-shot or few-shot learning*
4. *Joint multilingual learning*
  * Train a single model on a mix of datasets of all languages

**Paper**: [Choosing Transfer Languages for Cross-Lingual Learning](https://arxiv.org/pdf/1905.12688.pdf)

*how to define the similarity across languages ?*
* word overlap and sub-word overlap
* areal similairy: [www.glottolog.org](www.glottolog.org)
* demographic similarity
* genealogical similairy: [www.ethonologue.com](www.ethonologue.com)
* Typological similairy: explains commen properties or structural diversity
  [WALS](wals.info) - **Paper**:The World Atlas of Language Structures Online

### Automatic prediction of typological features
1. *Morphosynatctic annotation projection* - project feature annotations from similar Languages
2. *Unsupervised and semi-supervised feature propagation* - hierarchical typological clustering and majority value assignment / language-family based nearest neighbor projection/matrix completion
3. *Supervised learning* - Logistic regression/determinant point process with neural features
4. *Cross-lingual distribution feature alignment*

**Paper**:[Modeling language variation and universals: A survey on typological linguistics for natural language processing](https://arxiv.org/abs/1807.00914)
**Code**: URIEL(lang2vec: pypi.org/project/lang2vec)

### Linguistic universals
* all langs have vowels and consonants
* all langs of the world also make a distinction between nouns and verbs

### Linguistic typology in NLP

### Open research problems
* How to extract typological features automatically from existing multilingual resources
* How to accurately predict typological knowledge while controlling the bias
* how to incorporate linguistic typology into models
* how to alleviate negative transfer and catastrophic forgetting in multilingually trained models using typological knowledge
