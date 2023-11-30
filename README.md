# LLMsAnnotatingAntisemitism

## Annotation Task:

My project aims to investigate whether Large Language Models can be useful in identifying and annotating antisemitic statements on microblogging platforms. This task poses special challenges as contemporary antisemitism often manifests in veiled forms (e.g., relativizations instead of overt hostility) and is difficult to distinguish from non-antisemitic expressions (cf. Gessler 2006).

The basis for annotation is a detailed guideline built upon the definition provided by the International Holocaust Remembrance Alliance (IHRA). This definition has been endorsed and recommended by over 30 governments and international organizations, commonly used for monitoring and documenting antisemitic incidents. These guidelines were utilized in creating the dataset (cf. Jikeli et al. 2019).

## Dataset:

The dataset consists of a labeled set of 6,941 English tweets covering a range of topics where mentions of Jews, Israel, and antisemitic sentiments are expected (Jikeli 2023). The tweets were collected from January 2019 to December 2021 using representative samples with relevant keywords. The dataset also serves as an example for the annotation task and can be accessed here: https://doi.org/10.5281/zenodo.7932888. 
It was  published under the terms of the "Creative Commons Attribution 4.0 International" licence.

## LLM/Interface:

To conduct the annotation and compare the results of the LLM with those of human annotators, I propose using a chat-based interface due to the quantity of tweets to annotate. Instead, I'll use a locally deployed LLama.

## Experiment Design:

The experiment will utilize the already annotated data as a basis to compare the results of the LLM with those of human annotators. Their agreement will be evaluated using a Confusion Matrix. It is crucial to emphasize that success in this context only reflects agreement with human annotators and does not necessarily indicate the actual identification of antisemitic statements.
If necessary, manually testing particularly challenging examples is an option. Additionally, there is an opportunity to measure the influence of methods such as "Few Shot Prompting" on agreement.

The code of my experiment and all related data-collection and data-cleaning tasks will be provided in a jupyter notebook.

## Literature

Gessler, Philipp (2006). „Sekundärer Antisemitismus“. bpb.de, 21. https://www.bpb.de/themen/antisemitismus/dossier-antisemitismus/37962/sekundaerer-antisemitismus/.

Jikeli, Gunther, Damir Cavar, und Daniel Miehling (2019). „Annotating Antisemitic Online Content. Towards an Applicable Definition of Antisemitism“. https://doi.org/10.5967/3r3m-na89.

Jikeli, G., Karali, S., Miehling, D., & Soemer, K. (2023). Antisemitism on Twitter: A Dataset for Machine Learning and Text Analytics [Data set]. Zenodo. https://doi.org/10.5281/zenodo.7932888

Harden, Scott (2023): „Run Llama 2 Locally with Python“. Zugegriffen 27. November 2023. https://SWHarden.com.

