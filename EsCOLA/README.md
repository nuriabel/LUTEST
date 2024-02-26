Introduction

The Spanish Corpus of Linguistic Acceptability (EsCoLA) includes 11,174 sentences taken from linguistic literature with a binary annotation made by the original authors themselves. The work is inspired by CoLA: https://nyu-mll.github.io/CoLA/#


Paper


Núria Bel, Marta Punsola, Valle Ruíz-Fernández, 2024, EsCoLA: Spanish Corpus of Linguistic Acceptability. Joint International Conference on Computational Linguistics, Language Resources and Evaluation LREC-COLING 2024. Torino. Italy. 


Download


Download EsCoLA inDomain train and dev datasets, plus human annotation, from https://github.com/nuriabel/LUTEST/
For EsCoLA outDomain dataset and EsCoLA inDomain test data, please contact nuria.bel@upf.edu.


Data format


EsCoLA dataset is split into two subsets: an in-domain subset (InDomain) with 10,567 sentences, and an out-of-domain subset (OutDomain) with 607 sentences.
The in-domain subset has been split five times into train/dev/test sections: 
- train: 8454 sentences
- dev: 1053 sentences
- test: 1060 sentences
And the out-of-domain subset is split into dev/test sections. (no tenim la partició!!)
The test sets are not made public.

For the in-domain subset, each line in the .tsv files consists of 11 tab-separated columns:
- Column 1: a unique ID
- Column 2: the source of the sentence
- Column 3: the acceptability judgment label from the source (0=unacceptable, 1=acceptable)
- Column 4: the source's annotation (* for the unacceptable sentences)
- Columns 5, 6 and 7: the human annotations
- Column 8: the human annotations' median
- Column 9: the sentence
- Column 10: the category of the linguistic phenomenon the sentence is an example of
- Column 11: the split to which the sentence belongs

For the out-of-domain, each line in the .tsv file consists of 6 tab-separated columns:
- Column 1: a unique ID
- Column 2: the source of the sentence
- Column 3: the acceptability judgment label from the source (0=unacceptable, 1=acceptable)
- Column 4: the source's annotation (* for the unacceptable sentences)
- Column 5: the sentence
- Column 6: the category of the linguistic phenomenon the sentence is an example of


Corpus Sample


In-domain:


ID	Source	Label	Source_annotation	Annotator_1	Annotator_2	Annotator_3	Human_annotation_median	Sentence	Category	Split
EsCoLA_5681	GDE35	1		1	0	1	1	¿Opinaron si debían hacerlo?	7	train
EsCoLA_8872	GDE51	1		1	1	1	1	¿Quién ha llamado?	7	train
EsCoLA_5661	GDE35	1		1	0	0	0	No se sabe donde ir.	7	train
EsCoLA_7328	GDE42	0	*	0	1	1	1	Sólo tenía una peseta, y aquel tipo me pedía doscientos.	14	train

Out-of-domain:


ID	Source	Label	Source annotation	Sentence	Category
OD_1	ng34	1		El camino bordea el río.	1
OD_2	ng34	1		Las aves vuelan.	1
OD_3	ng34	1		Pepe tiene dinero.	1
OD_4	ng34	1		Tengo hambre.	1
OD_5	ng34	0	*	Dudo tu solución.	1



Processing


During gathering of the data and processing, some sentences from the source documents may have been omitted or altered. We discarded examples marking dubious acceptability with "?" or other signs, but those examples that included acceptability alternations were taken by creating the two versions: the acceptable and the unacceptable sentence. Finally, the examples that were not
full sentences, that is, that contain no main verb, were manually edited to add a neutral verb to convert them into sentences, while keeping the acceptability value.


Sources


Demonte and Bosque (1999)-InDomain
RAE (2009)-OutDomain
Palencia and Aragonés (2007)-OutDomain
Díaz and Yagüe (2019)-OutDomain

Annotation
The dataset has been manually annotated with 14 linguistic phenomena.
1. Simple
2. Predicative
3. Adjuncts
4. Argument types
5. Argument alternation
6. Binding pronouns
7. Wh-phenomena
8. Complement clauses
9. Modal, negation, periphrasis and auxiliaries
10. Infinitive embedded VPs and referential phenomena
11.Complex NPs and APs
12. S-Syntax
13. Determiners, quantifiers, comparative and superlative constructions
14. Spanish phenomena
The Spanish phenomena have been classified into 6 categories:
1. Agreement in nominal constructions
2. Subjunctive mode and tense
3. Spurious preposition for completive clauses ('dequeismo')
4. Subject ellipsis
5. Pronominal cliticization
6. Ser/estar copula selection

Citation

Please, if you use the dataset cite the following papers:

Alex Warstadt, Amanpreet Singh, and Samuel R. Bowman. 2018. Neural network acceptability judgments. arXiv preprint arXiv:1805.12471.

Núria Bel, Marta Punsola, Valle Ruíz-Fernández, 2024, EsCoLA: Spanish Corpus of Linguistic Acceptability. Joint International Conference on Computational Linguistics, Language Resources and Evaluation LREC-COLING 2024. Torino. Italy. 


Disclaimer


The dataset has been made copying the examples from published works that are protected by copyright. According to the anonymized law, we have respected the copyright because the number of elements taken represent less than a 10% of the whole work, and the number of items copied is justified by the aims of research.
