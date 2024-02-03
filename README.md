# Assign_ICL

**S1 CL and Definition**
1. **Definition of Computational Linguistics**  
Brings computer and languages together. The specific study of language from a computational perspective. The study of of computer systems for understanding and generating natural language.
2. **Aims of the field**: To get computers to perform human language tasks.
3. **Different characteristics and applications**  
Sentimen analysis, dialogue system, speech recognition, machine translation, etc.
4. **Different perspectives (theory, methods, tasks)**  
- _Theory_: Describing content and format of descriptions of phenomena, including formulating abstract models/frameworks to understand underlying pricinciples governing language structures and behaviours. _Understanding_
- _Methods_: Developing tools, procedures, formalism to facilitate NLP/ML by creating algorithms/models. _Modeling_
- _Tasks_: applying methods to solve specific language tasks. _Utilising_
5. **Different methodologies (rule-based, statistical approaches)**  
- _Rule-based approaches_: Explicitly model language by defining set of linguistic rules and structures crafted by human experts. Reply on predefined sets of linguisitcs rule. Transparent, interpretable, but labour-intensive and struggle from complexity.
- _Statistical approaches_: Implicitly model language based on patterns and probabilities derived from large datasets, leaveraging statisitcal models and ML algorithms to learn these patterns. Handles complexity, struggle from limited training data.
- _How language is related to this_: Language is rule-govened yet shows statistical regularities. Rule-based capture explicit linguistic features, statistical embrace implicit statistical patterns. The interplay between them reflects the multidimensional nature of language in computational modeling.
6. **Relation to General Linguistics**
- GL is the study of human language as a universal and recognasible part of human behaviours and cognitive abilities.
- Common foundation in exploration of language
- Approches and Outlook: GL looks at all languages' universals and principles, CL deals more specifically with the technological aspects of language processing. GL covers entirety of human languages. CL focuses on pratical applications and the development. GL - theoretical foundations, CL - real application.
- CL can be viewed as an applied subset of GL, theoretical insights from the latter guide the CL models for practical language-specific tassks. Altogther contribute to our understanding of language.
7. **Main subtasks in NLP (NLU, NLG)** 
- NLU: mapping given NL input into useful representations, analysing different aspects of the input: lexicon (POS tagging), morphology (lemmatization), syntax (dependency parsing), discourse (anaphora resolution), pragmatics (sentiment detection).
- NLG: producing meaning natural language text from some more abstract representation: subtle (difficult to get it right), very domain-specific (systems are tailored to particular applications/tasks: e.g. generating weather reports vs. poems).


**S2 Encoding Language**
**Writing Systems**
- Alphabetic, Syllabic, Logographic 
How is language encoded on computers? (bits & bytes) 
Binary and Hexadecimal System 
Binary system is base 2, using the symbols 0 and 1 01101=0∗24+1∗23+1∗22+0∗21+1∗20 =13
Hexadecimal system is base 16, the numbers 0 to 9 and the letters A (=10) to F(=15)2are used 1 0
0xA8E=10∗16 +8∗16 +14∗16 =2702
Conversion: 4 positions in binary can be represented with 1 position in hexadecimal 
ASCII
ASCII uses 8 bits to store 256 characters, was developed for the Latin Alphabet (esp. English)
Served as basis for future encoding systems
You should be able to read and use the ASCII chart You should be able to discuss the necessity of a standardised coding table & the limitations of ASCII 
Unicode
Uses (up to) 32 bits 
has a single representation for every character UTF-8 allows for backwards compatibility with ASCII UTF-8 allows for variable length (first bits show how many bytes are used) 
0 ... → one byte
110... → two bytes (following: 10..) ... 
You should be able to discuss the advantages and limitations of unicode 


S3: Writers’ Aids 
Spelling variation (regional differences, different genres) 
Spelling error types (non-word, real-word errors)
Error sources (opaque writing systems, L1 transfer, etc.) 
Basic edit operations (I, D, S, T) 
High-level stages in method for automatic spell checking (detection, generation, ranking) 
Information sources for different stages: 
Detection: word lists 
Generation: a) rules b) list of valid words & similarity measures Ranking: explain why ranking is needed 
Minimal String Edit Distance (concept and algorithm) 
Operatilising string similarity with naive examples 
Modelling string similarity after human typist operations 
Why DAGs are useful tool for representing search space 

S4: Text as Data
What is a Corpus?
Structured collection of texts collected with a specific question in mind. Usually contains linguistic annotation and metadata 
What is Metadata?
Data describing the primary, ra data (creation date, information and the speaker/writer/author, tags, ...) 
What are Linguistic Annotation
POS tags, sentence/word boundaries, parse trees, ... 
TTR = #types #tokens 
Limitations & applications of corpora 
You should be able to discuss whether a certain corpus is appropriate for a specific research question, what the steps would be to collect data, what kind of (meta) data would be necessary to answer a certain RQ... 

S5 Text Classification
How computers learn 
Feature vectors 
Training, Testing, Validation Set 
Supervised vs. Unsupervised ML 
Supervised: Labeled data through expert annotators. 
1) Split the data
2) train the model
3) test and cross-validate
4) evaluate 
Unsupervised: 
1) feature extraction
2) apply algorithm on dataset
3) inspect resulting structure 
How to evaluate a model
Recall, Precision, Accuracy, TNR
How are these calculated?
When should you use which measure? → Is it more important to catch everyone with the disease and maybe treat healthy patients, or is it better to miss some patients but be sure not to treat healthy people? Is it better to censor non-harmful tweets and make sure to censor every hate speech tweet ... ? 
4. NLP segmentation
Preprocessing
Tokenisation: What is a token, what are the challenges (contracted forms, hyphenated forms, periods (St.), special characters, NER, …)
Sentence segmentation: How are sentences defined, what are the challenges in sentence segmentation (esp. with regards to other languages than English)

S6 ASR
Brief introduction to speech (phones and phonemes, vocal tract)
How speech is represented with computers
Different speech processing applications
Which ones can you think of?
What task does each one perform?
What language technology components are required in the pipeline to make these applications work?
4. Automatic speech recognition
Inputs/Outputs
Why ASR is a difficult problem
Noisy channel model and application to ASR
System architecture of ‘classical’ ASR system; role of components (acoustic model, lexicon, language model, search lattice, decoder)
Purpose of language model
Using a language model to rank different candidates (“wooden boats”)
A very high-level look at probabilities (coin flipping) and n-gram language models
Steps in training a speech recogniser (dataset requirements, feature extraction, training, testing, evaluation, error analysis)


S7 Text Search
Why search can be challenging, with example(s)
Different search tasks (hint: Google, Quora, Netflix)
Key terms, such as information need, intent, query
Formulating queries: general user vs. specialist user
Regular expression
Definition 
Basic building blocks:
Literals
Wild cards
Escaping
Modes (/g, or /i)
Character sets and ranges
Quantified repetition
Groups using parentheses
Anchors
Multiple Documents
Examples of applications searching multiple documents
What document indexing is, why it is important, and different approaches (term-by-document matrix, inverted indices list)
Evaluating search quality
User experience surveys
Objective user interaction logs
Precision, Recall (and challenges with computing recall), F-measure
An understanding of the limitations of these measures in the context of Text Search
An understanding of why Ranking is important in text search

S8 CALL
Characteristics of learner language (in contrast to native-like language) and implications for NLP technology
Know what an Intelligent Tutoring System (ITS) is 
Be able to talk about NLP applications in the context of ITS for language learning
NLP applied to well-formed language (e.g. FLAIR)
NLP applied to malformed learner language
For each, be able to describe:
The needs of the users (e.g., input, corrective feedback)
How NLP can be used in an ITS to meet those needs
Using knowledge from other lectures (e.g. text search), make suggestions for how to evaluate the quality of an NLP-enhanced ITS system


S9 Dialogue Systems
Terminology
Speech acts, common ground, turn taking, adjacency pairs
How are these important for dialogue systems?
Grice’s Maxims
What are they, how are they defined?
Why are they important in dialogue systems? What happens if they are not met?
Task Specific Systems
Designed to help accomplish one or more specific tasks
Intents containing slots, intent recognition
Independent Systems
Chatbots
Different implementations (brute force, rule-based, corpus trained, generative)
You should be able to explain the previously mentioned phenomena on chatbot examples (e.g. explain the rule based approach on the example of ELIZA)
How are chatbots evaluated? (Turing test, Winograd Schemas)
POS tagging
Information on word type (noun, verb, etc)
Different granularity depending on corpus
Used to encode morphological and syntactical information of tokens, can be used to measure linguistic properties such as complexity o pronunciation
Often prerequisite for other NLP tasks
Methods for POS tagging
Rule-based
Use constraint grammars and lexicons to retrieved all candidate POS tags and the associated rules
They each rule on input sentence and exclude POS tag if tule does not fit
Statistical
Input a token sequence, assign a POS tag to each token, handle ambiguity by exploring different possible sequences
Rank each sequence by its statical probability using supervised ML
Challenges in POS tagging
Ambiguity
Sometimes, various POS tags are possible (I can can a can of tuna) - context necessary
You should be able to annotate short sequences and discuss possible ambiguities including ways to resolve the ambiguity
Parsing
Represent grammatical structures or relationships
Constituency Parsing
Constituents: Group of words forming syntactic units (e.g. NPs)
Parsing assigns syntactic structures
Identification of multi-word units and nested structures
Visualisations: Trees and parentheses notation. You should be able to read & create both forms
Challenge: Ambiguities, e.g. I saw the man with the telescope
Dependency Parsing
Aim: Capture the syntactic relations between words in a sentences using directed grammatical relation between pairs of words
Relation have governor (head) and dependent 
Challenges: Attachment and corrpdinasion ambiguity
S10 LLMs
Technical Aspects
You do not need to be able to explain what neural networks are or what a transformer is, but you need to know the vocabulary!
You should be able to discuss what was new about LLMs (one model for all, parallelisation, attention)
Large Language models
Applications of LLMs
You should be able to name a few applications of LLMs
Ethical Aspects
Bias
Difficulty of unbalanced, restricted, and biased corpora
How are social biases inscribed in the data?
Why is this problematic?
Fine tuning
Why is it difficult to ensure that only ‘ethical’ utterances are generated?
How did chatbots try to solve this problem? How is it done nowadays?
Environment impact
You should be able to shortly discuss possible environmental impacts (also considering the large datasets, long learning etc.)




