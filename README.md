# EHRI-NER

## Dataset Card for ehri-ner/ehri-ner-all

<!-- Provide a quick summary of the dataset. -->
The European Holocaust Research Infrastructure (EHRI) aims to support Holocaust research by making information
about dispersed Holocaust material accessible and interconnected through its services. Creating a tool capable of
detecting named entities in texts such as Holocaust testimonies or archival descriptions would make it easier to
link more material with relevant identifiers in domain-specific controlled vocabularies, semantically enriching it, and
making it more discoverable. The EHRI-NER dataset is a multilingual dataset (Czech, German, English, French, Hungarian, Dutch, Polish, Slovak, Yiddish) 
suitable for training domain-specific Named Entity Recognition (NER) models for Holocaust-related texts.  

We have converted all available Extensible Markup Language (XML) files from the EHRI digital scholarly
editions (i.e., EHRI Online Editions) into a corpus in a format
suitable for training NER models. 

## Dataset Details

The EHRI-NER dataset includes a total of
505758 tokens, with 5351 person entities, 9399
location entities, 1867 organization entities, 2237
date entities, 528 ghetto entities, and 1229 camp
entities.


### Dataset Description

<!-- Provide a longer summary of what this dataset is. -->

Since 2018, the EHRI Consortium has supported
the development and publication of six
Holocaust-related digital scholarly editions (see [here](https://www.ehri-project.eu/ehri-online-editions)). 
Each edition enables digital access to facsimiles
and transcripts of thematically related documents
held by different EHRI partner institutions
through a single web interface and unlocks new
ways of presenting and browsing through historical
sources using digital tools. Publishing a digital
edition is a resource-intensive process. Notwithstanding
the extensive archival research needed
for selecting the documents, additional steps include
transcribing and translating them and, most
importantly, annotating words and phrases found
within these texts and creating links with entities in
controlled vocabularies provided by EHRI and third
parties. Currently, this annotation is done manually
by or under the supervision of subject matter experts,
ensuring a high quality of annotations. We
repurposed these resources to convert them into
a dataset suitable for training NER models, which
we consider as a gold standard.  

Each EHRI Online Edition consists of digitized
documents originating from various archives that
are selected, edited, and annotated by EHRI researchers
using the Text Encoding Initiative (TEI)
P5 standard (TEI Consortium, 2023), an XML
schema, which supports their online publication.
Editions enhance the edited documents by contextualizing
the information contained within them and
linking them to EHRI vocabularies and descriptions,
and by visualizing georeferenced entities through
interactive maps. Thanks to their encoding in TEI,
they are fully searchable and can be filtered using
facets such as spatial locations, topics, persons, organizations,
and institutions. All documents within
an edition have a transcript, either in their original
language, a translation, or both, and have access
to their facsimile. EHRI Editions are published without
a regular schedule and it is possible to update
them with new material or improve the already published
documents.  

The resulting EHRI-NER
dataset includes nine languages: Czech (cs),
German (de), English (en), French (fr), Hungarian
(hu), Dutch (nl), Polish (pl), Slovak (sk), and Yiddish
(yi).

- **Curated by:** EHRI
- **Funded by:** European Commission call H2020-INFRAIA-2018–2020. Grant agreement ID 871111. DOI 10.3030/871111.
- **Shared by:** Dermentzi, M. & Scheithauer, H.
- **Language(s) (NLP):** cs, de, en, fr, hu, nl, pl, sk, yi
- **License:** EUPL-1.2

<!-- ### Dataset Sources



- **Repository:** https://github.com/EHRI/EHRI-NER
- **Paper:** [More Information Needed]
 -->
## Uses

<!-- Address questions around how the dataset is intended to be used. -->
EHRI-NER is a multilingual dataset (Czech, German, English,
French, Hungarian, Dutch, Polish, Slovak, Yiddish) for Named Entity Recognition (NER) in Holocaust-related texts.
EHRI-NER is built by aggregating all the annotated documents in the EHRI Online Editions and converting them into a
format suitable for training domain-specific NER models.


### Source Data

<!-- This section describes the source data (e.g. news text and headlines, social media posts, translated sentences, ...). -->
This dataset is derived from the EHRI Online Editions, a series of six Holocaust-related digital scholarly editions (more info [here](https://www.ehri-project.eu/ehri-online-editions)). 


#### Who are the source data producers?

<!-- This section describes the people or systems who originally created the data. It should also include self-reported demographic or identity information for the source data creators if this information is available. -->

This dataset
was made possible thanks to the previous work
of the editors and contributors of the EHRI Online
Editions, including the annotators, the people who
produced digital facsimiles of the original archival
material, and those who created the transcripts
and translations.


## Bias, Risks, and Limitations

<!-- This section is meant to convey both technical and sociotechnical limitations. -->
This dataset stems from a series of manually annotated
digital scholarly editions, the EHRI Online Editions. The original purpose
of these editions was not to provide a dataset
for training NER models, although we argue that they nevertheless
constitute a high-quality resource that is
suitable to be used in this way. However, users should still be mindful that 
our dataset repurposes a resource that was not built for purpose.  

This dataset was put together as part of an EHRI-specific research project and may not be suitable for 
the purposes of other users/organizations.

<!-- ### Recommendations

We encourage potential users to read the paper accompanying this model before deciding to use this dataset for their purposes:  

Dermentzi, M., & Scheithauer, H. (2024, May 21). Repurposing Holocaust-Related Digital Scholarly Editions to Develop Multilingual Domain-Specific Named Entity Recognition Tools. Proceedings of the LREC-COLING 2024 Workshop on Holocaust Testimonies as Language Resources. HTRes@LREC-COLING 2024, Turin, Italy.

## Citation

**BibTeX:**
@inproceedings{dermentzi_repurposing_2024,
	address = {Turin, Italy},
	title = {Repurposing {Holocaust}-{Related} {Digital} {Scholarly} {Editions} to {Develop} {Multilingual} {Domain}-{Specific} {Named} {Entity} {Recognition} {Tools}},
	booktitle = {Proceedings of the {LREC}-{COLING} 2024 {Workshop} on {Holocaust} {Testimonies} as {Language} {Resources}},
	author = {Dermentzi, Maria and Scheithauer, Hugo},
	month = may,
	year = {2024},
    pubstate={forthcoming},
}


**APA:**
Dermentzi, M., & Scheithauer, H. (2024, May 21). Repurposing Holocaust-Related Digital Scholarly Editions to Develop Multilingual Domain-Specific Named Entity Recognition Tools. Proceedings of the LREC-COLING 2024 Workshop on Holocaust Testimonies as Language Resources. HTRes@LREC-COLING 2024, Turin, Italy.

 -->
