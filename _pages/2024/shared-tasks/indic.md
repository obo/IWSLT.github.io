---
permalink: /2024/indic
title: "Indic track"
toc: true
toc_sticky: true
---

<!--
Markdown notes: comments can be formed as in this example;
bulleted lines start with a - ;
if you want to have a line break either put a blank line in between the text or leave two spaces at the end of the line
-->

## Description

In the realm of spoken language processing, Speech-to-Text Translation (ST) holds a crucial role at the intersection of natural language processing. The primary aim of ST is to convert spoken language from one linguistic context into written text in another language. This typically involves using Automatic Speech Recognition (ASR) to convert speech in the source language into text, followed by Machine Translation (MT) to translate the source language text into the target language. ST is a multimodal task that takes speech input and produces output in text format. Furthermore, it is inherently multilingual, taking speech input in one language and generating text output in another.Traditionally, human language translators proficient in both the source and target languages have handled this task. However, the scarcity of translators fluent in multiple languages has created a pressing need for a dedicated model tailored to excel in the unique realm of ST tasks across diverse languages. Recent advancements in ST have predominantly focused on high-resource languages, leaving a significant gap for low-resource languages that face a substantial catch-up journey. The attention imbalance is primarily due to the scarcity of data for low-resource languages, as most deep-learning models depend on data abundance. Acquiring such data for low-resource languages poses a formidable challenge.

While a considerable body of research is dedicated to ST across diverse language families, there is a noticeable gap in investigating this domain concerning low-resource Indian languages. Currently, there are no datasets specifically designed for the ST task in Indian languages, covering both the Indo-Aryan and the Dravidian language families. The goal of this research is to create an End-to-End (E2E) Speech-to-Text (ST) model that encompasses all Indian languages.

The aim of this Indic-track shared task is to establish a speech translation model that spans a diverse array of dialects and low-resource languages originating from the Indo-Aryan and Dravidian language families in India. Given that a significant portion of the data is sourced from very low-resource languages, these languages remain largely unexplored in the realm of speech translation. Compounding this challenge is the fact that many of the target languages are distantly related to English. Consequently, we anticipate that relying solely on pre-trained models may encounter numerous obstacles. The dataset provided will serve as the inaugural benchmark and gold standard dataset, encompassing all major Indian languages. Our aspiration is for participants to develop systems capable of real-world deployment in the future.

<!-- Description the task, the languages, and the type of data -->

## Data & Baselines

The ST task data for the Indic-track will encompass three Indian languages representing diverse language families. The languages included in this shared task are Hindi (hi), Bengali (bn), and Tamil (ta), originating from the Indo-Aryan and Dravidian language families. The dataset will include speeches and texts (transcriptions) in English (source language) and texts (translations) in Hindi, Bengali, and Tamil (target languages).

The data for this Indic-track shared task comprises a Speech-to-Text (ST) corpus that includes 3 low-resource Indian languages. Table 1 illustrates the consistency maintained across all corpora, with an equal number of lines in their .en, .lang, and .yaml files. However, due to inherent linguistic differences, the number of tokens in the .en and .lang files varies. The count of audio files corresponds to the number of distinct talks, each delivered by an individual speaker. Additionally, the speech hours indicate the cumulative duration of speech in a given language. Each of these parameters is meticulously categorized into test, train, and valid subsets, establishing a comprehensive and structured dataset.

<!-- Details description of the data and links to download -->

#English to Hindi (en-> hi): 

Hindi is the third most spoken language in the world, with 615 million speakers. It belongs to Indo-Aryan language family, mainly spoken in India. It is also the official language of India, written in Devnagiri script. The data contains English speech, English texts (transcripts), and Hindi texts (translations). The speech of English language is 95.7 hours and the texts for Hindi language is 37K lines. The data is available here. 

The baseline for English to Hindi speech translation is a BLEU score of 5.23.

#English to Bengali (en-> bn): 

Bengali is the 7th most spoken language in the world, with 228 million speakers. It belongs to Indo-Aryan language family, spoken in Bengal region of South-Asia. It is also the official language of Bangladesh, written in Bengali-Assamese script. The data contains English speech, English texts (transcripts), and Bengali texts (translations). The speech of English language is 16.44 hours and the texts for Bengali language is 6.9K lines. The data is available here. 

The baseline for English to Bengali speech translation is a BLEU score of 5.86.

#English to Tamil (en-> ta): 

Tamil is one of the classical languages of India, spoken by 90.8 million speakers. It belongs to Dravidian language family, spoken by Tamil people of South-Asia. It is the official language of Tamil Nadu state of India, written in Brahmi script. The data contains English speech, English texts (transcripts), and Tamil texts (translations). The speech of English language is 22.15 hours and the texts for Tamil language is 8K lines. The data is available here. 

The baseline for English to Tamil speech translation is a BLEU score of 1.9.

<!-- ## Baselines -->

<!-- Links to the baselines to be used (descriptions, publications and/or links to models, code) -->

##Conditions:

The submissions for the all the language-pairs can for the below 2 conditions:

1. Constrained Conditions: Only the language data provided with the data here can be used for pre-training the models. No data from any other sources can be used for pre-training of the models. 


2. Unconstrained Conditions: Any pre-trained models and any other data can be used for pre-training the models. 


## Submission

<!-- Description of expected submission format and submission instructions -->
The submissions must be mailed to this email:

Only one submission is allowed per team. 

The submissions must be submitted zipped in tar.gz format and then emailed. 

The email should include the following information:

Institute:
Contact Person:
Email:
Data condition: Constrained/Unconstrained
Segmentation: Own/Given
Brief abstract about the system:
Multilingual: Yes/No
Do you want to make your submissions freely available for research purposes? (yes/no)


## Evaluation

<!-- Description of metrics used for evaluation, what the official ranking is based on, links to evaluation scripts -->
Only one test-set will be provided for each language-pair, consisting Speech in the English language only. 

## Organizers

<!-- List of organizers' names and affiliations -->

1. Nivedita Sethiya (PhD Scholar, AI Lab, Computer Science and Engineering, Indian Institute of Technology Indore, India)- phd2201201003@iiti.ac.in
2. Balaram Sarkar (MS, AI Lab, Computer Science and Engineering, Indian Institute of Technology Indore, India)- ms2204101006@iiti.ac.in
3. Dr. Chandresh Kumar Maurya (Assistant Professor, AI Lab, Computer Science and Engineering, Indian Institute of Technology Indore, India)- chandresh@iiti.ac.in

## Contact

<!-- Add chair(s) and their contact info, as well as standard google group -->
Chair:   
Discussion: <iwslt-evaluation-campaign@googlegroups.com>