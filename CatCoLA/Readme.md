
 
GENERAL INFORMATION
------------------

1. Dataset title:

CatCoLA - Catalan Corpus of Linguistic Acceptability


2. Authorship:

	Name: Núria Bel
	Institution: Universitat Pompeu Fabra, UPF
	Email: nuria.bel@upf.edu
	ORCID:  0000-0001-9346-7803

	Name: Marta Punsola
	Institution: Universitat Pompeu Fabra, UPF
	Email: marta.punsola@gmail.com
	ORCID:  

	Name: Valle Ruiz-Fernández
	Institution: Barcelona Supercomputing Center
	Email: valle.ruizfernández@bsc.es
	ORCID:  

DESCRIPTION
----------

1. Dataset language:

Catalan


2. Abstract:

We introduce CatCoLA, the Catalan Corpus of Linguistic Acceptability that will contribute to the Catalan Language Understanding Benchmark (CLUB) to assess and compare the capabilities of language models (LM) trained with texts in Catalan. CatCoLA follows the design of the English CoLA to support the task of classifying sentences as acceptable or not. CatCoLA consists of 10,443 sentences and their acceptability judgements as found in well-known Catalan reference grammars. Additionally, all sentences have been annotated with the class of linguistic phenomenon the sentence is an example of, also following previous practices. CatCoLA is released under a CC BY-NC-SA 4.0 licence and freely available at https://github.com/nuriabel/LUTEST

3. Keywords: 
Language model evaluation, corpus of linguistic acceptability, Spanish


4. Date of data collection (single date or date range):

2023

5. Publication Date:

29-05-2024


6. Grant information:
This research is part of the LUTEST project, PID2019-104512GB-I00, funded by the Ministerio de Ciencia, Innovación y Universidades and Agencia Estatal de Investigación (Spain). BSC participation has been promoted and financed by the Generalitat de Catalunya through the Aina project and by the Ministerio para la Transformación Digital y de la Función Pública and Plan de Recuperación, Transformación y Resiliencia - NextGenerationEU within the framework of the project ILENIA (2022/TL22/00215337-00215334).

7. Geographical location/s of data collection:

Spain



ACCESS INFORMATION
------------------------

1. Creative Commons License of the dataset:
CC-BY-NC-SA, Creative Commons Attribution 4.0 International License

2. Dataset DOI:

pending


3. Related publication:

Núria Bel, Marta Punsola, Valle Ruíz-Fernández, 2024, CatCoLA: Catalan Corpus of Linguistic Acceptability.  Procesamiento del Lenguaje Natural 73, 2024.

4. Link to related datasets:

https://github.com/nuriabel/LUTEST


VERSIONING AND PROVENANCE
---------------

1. Last modification date:

19-05-2024

2. Were data derived from another source?
The dataset has been made copying the examples from published works that are protected by copyright. According to the Spanish law, we have respected the copyright because the number of elements taken represent less than a 10% of the whole work, and the number of items copied is justified by the aims of the research.




3. Additional related data not included in this dataset:
[Optional]


METHODOLOGICAL INFORMATION
-----------------------
See the paper


Download

Download CatCola train and dev datasets, plus human annotation, from https://github.com/nuriabel/LUTEST/

For CatCola outDomain dataset and CatCoLA inDomain test data, please contact nuria.bel@upf.edu.


Data format

CatCoLA dataset is split into two subsets: an in-domain subset (InDomain) with 10,189 sentences, and an out-of-domain subset (OutDomain) with 254 sentences.

The in-domain subset has been split into train/dev/test sections: 
- train: 8151 sentences
- dev: 1018 sentences
- test: 1020 sentences

The test sets are not made public to avoid contamination. Please write nuria.bel@upf.edu. 

For the in-domain subset, each line in the .tsv files consists of tab-separated columns:
- Column 1: a unique ID
- Column 2: the source of the sentence
- Column 3: the acceptability judgment label from the source (0=unacceptable, 1=acceptable)
- Column 4: the source's annotation (* for the unacceptable sentences)
- Columns 5, 6 and 7: the human annotations
- Column 8: the sentence
- Column 9: the category of the linguistic phenomenon the sentence is an example of
- Column 10: the split to which the sentence belongs

For the out-of-domain, each line in the .tsv file consists of tab-separated columns:
- Column 1: a unique ID
- Column 2: the source of the sentence
- Column 3: the acceptability judgment label from the source (0=unacceptable, 1=acceptable)
- Column 4: the source's annotation (* for the unacceptable sentences)
- Column 5: the sentence
- Column 6: the category of the linguistic phenomenon the sentence is an example of



Processing

During gathering of the data and processing, some sentences from the source documents may have been omitted or altered. We discarded examples marking dubious acceptability with "?" or other signs, but those examples that included acceptability alternations were taken by creating the two versions: the acceptable and the unacceptable sentence. Finally, the examples that were not full sentences, that is, that contain no main verb, were manually edited to add a neutral verb to convert them into sentences, while keeping the acceptability value.

Sources

- InDomain
Abril, Joan (1997). Diccionari pràctic de qüestions gramaticals. Barcelona: Edicions 62. Nova ed., 2010. Barcelona: Educaula.
Abril, Joan; Riera, Elvira (1997). L’ús dels possessius. Llengua i Ús (Barcelona), n. 10, p. 32-36. 
Abrines, Bartomeu (2011). Els verbs de canvi d’estat en català: la participació en l’alternança causativa. Caplletra (València), n. 50, p. 35-65. 
Albareda, Cristina (2013). La duplicació pronominal en les relatives locatives en català. Zeitschrift für Katalanistik (Friburg, Bochum), v. 26, p. 275-299. 
Ballesta, Joan-Manuel (1987). Algunes consideracions entorn dels verbs copulatius en català. Llengua & Literatura (Barcelona), n. 2, p. 359-375. 
Bartra, Anna (2016). Els components de la passiva. Una perspectiva diacrònica. Caplletra (València), n. 61, p. 295-327. 
Bartra, Anna; Brucart, Josep Maria (1982). Alguns arguments a favor de la categoria sintagma predicatiu. Els Marges (Barcelona), n. 24, p. 91-113. 
Busquets, Joan (2006). Stripping vs. VP ellipsis in Catalan: what is deleted and when? Probus (Dordrecht), v. 18, n. 2, p. 159-187. 
Cuenca Ordinyana, Maria Josep (2006), La connexió i els connectors. Perspectiva oracional i textual. Vic. Eumo Editorial.
Cuenca Ordinyana, Maria Josep (2012), Sintaxi catalana. Barcelona: Editorial UOC: 
Espinal, M. Teresa (2000). Sobre les expressions lexicalitzades. Els Marges (Barcelona), n. 67, p. 7-31.
Espinal, M. Teresa (2010). Bare nominals in Catalan and Spanish. Their structure and meaning. Lingua (Amsterdam), v. 120, n. 4, p. 984-1009.
Generalitat de Catalunya. Departament de Justícia. Curs de llengua catalana. Nivell C. 
Hernanz, M. Lluïsa; Rigau, Gemma (1984). Auxiliaritat i reestructuració. Els Marges (Barcelona), n. 31, p. 29-51. 
Mascaró, Joan et al. (1984) Estudis gramaticals. Bellaterra: Universitat Autònoma de Barcelona, p. 109-148. 
Portal del Consorci per la normalització lingüística: https://www.cpnl.cat/gramatica/
Rigau, Gemma (1990). Les propietats d’“agradar”: estructura temàtica i comportament sintàctic. Caplletra (València), n. 8, p. 7-19. 
Rigau, Gemma (1993). El comportamiento sintáctico de los predicados existenciales en catalán. Revista de Lenguas y Literaturas Catalana, Gallega y Vasca (Madrid), v. 3, p. 33-53. 
Rigau, Gemma (1994). Les propietats dels verbs pronominals. Els Marges (Barcelona), n. 50, p. 29-39.
Solà, Jaume (2002). Clitic climbing and null subject languages. Catalan Journal of Linguistics (Bellaterra), v. 1, p. 225-255.
Solà, Joan; Lloret, Maria-Rosa; Mascaró, Joan; Pérez Saldanya, Manuel (dirs.) (2002). Gramàtica del català contemporani. Amb la col·laboració de Gemma Rigau. 4a ed., definitiva, 2008. Barcelona: Empúries.
Viana, Amadeu (1990). La sintaxi de la conjugació en català. Caplletra (València), n. 8, p. 81-105.
Villalba, Xavier (1992). Case, incorporation, and economy: an approach to causative constructions. Catalan Working Papers in Linguistics (Bellaterra), v. 2, p. 345-389. 
Villalba, Xavier (1994a). Clitic climbing in causative constructions. Catalan Working Papers in Linguistics (Bellaterra), v. 3, n. 2, p. 123-152.
Villalba, Xavier (1994b). Clitics, case checking, and causative constructions. Kansas Working Papers in Linguistics (Kansas), v. 19, n. 1, p. 125-147. 
Villalba, Xavier (2004). Descripció i norma: amb i el canvi de preposició. Llengua \& Literatura (Barcelona), n. 15, p. 257-276. 


- OutDomain
Pisani, M.; Zevallos, R.; Bel, N. (2023). Catalan Parliamentary Plenary Session Transcriptions from 2015 to 2022, the ParlaMintCAT Corpus. Procesamiento del lenguaje natural, 71. 

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
14. Catalan phenomena
The Catalan phenomena have been classified into 7 categories:
1. Agreement in nominal constructions
2. Subject ellipsis
3. Ser/estar copula selection
4. Constructions with the hi pronoun
5. Pronominal cliticization
6. Subjunctive mode and tense and consecutio temporum
7. Dislocation

Citation

Please, if you use the dataset cite the following papers:

Alex Warstadt, Amanpreet Singh, and Samuel R. Bowman. 2018. Neural network acceptability judgments. arXiv preprint arXiv:1805.12471.

Núria Bel, Marta Punsola, Valle Ruíz-Fernández, 2024, EsCoLA: Spanish Corpus of Linguistic Acceptability. Joint International Conference on Computational Linguistics, Language Resources and Evaluation LREC-COLING 2024. Torino. Italy. 
 

Disclaimer

The dataset has been made copying the examples from published works that are protected by copyright. According to the Spanish law, we have respected the copyright because the number of elements taken represent less than a 10% of the whole work, and the number of items copied is justified by the aims of research.


