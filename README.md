# Authors
Davide Varagnolo (d.varagnolo@studenti.unipi.i), Department of Informatics, University of Évora, Portugal and NOVA Laboratory for Computer Science and Informatics, NOVA LINCS, Portugal

Dora Melo (dmelo@iscac.pt), Coimbra Business School | ISCAC, Polytechnic Institute of Coimbra, Portugal, CEOS.PP Coimbra, Polytechnic Institute of Coimbra, Portugal, and NOVA Laboratory for Computer Science and Informatics, NOVA LINCS, Portugal

Irene Pimenta Rodrigues (ipr@uevora.pt), Department of Informatics, University of Évora, Portugal and NOVA Laboratory for Computer Science and Informatics, NOVA LINCS, Portugal


# PartialDRSBuilder
The partial DRS builder tool receives a natural language sentence and translates it into a Partial DRS.

The PartialDRS-code.zip contains the Java code of the partial DRS builder tool (part of a Maven Java project).

## Query Ontology

Query Ontology (QueryOntology.rdf) represents the natural language concepts conveyed by the questions used to query the DBLP RDF knowledge base.

## Question Dataset

The dataset-100questions.tsv is organized as follows:
* qN = question number
* qID = question identifier of DBLP-QuAD (https://huggingface.co/datasets/awalesushil/DBLP-QuAD)
* type = type of question (single or multi fact) of DBLP-QuAD (https://huggingface.co/datasets/awalesushil/DBLP-QuAD)
* question = natural language question or rephrased question of DBLP-QuAD (https://huggingface.co/datasets/awalesushil/DBLP-QuAD)
* template-id = template identification assigned by DBLP-QuAD (https://huggingface.co/datasets/awalesushil/DBLP-QuAD)

## Evaluation of the Question-Answering System answer

The "evaluation dataset.tsv" ("evaluation dataset.xlsx") is organized as follows:
* qN = question number
* qID = question identifier of DBLP-QuAD (https://huggingface.co/datasets/awalesushil/DBLP-QuAD)
* type = type of question (single or multi fact) of DBLP-QuAD (https://huggingface.co/datasets/awalesushil/DBLP-QuAD)
* question = natural language question or rephrased question of DBLP-QuAD (https://huggingface.co/datasets/awalesushil/DBLP-QuAD)
* DRS-question = question Partial DRS 
* DRS-Ont-question = question final DRS
* SPARQL-question = SPARQL query generated from question final DRS
* Result-question = evaluation result (0 - Stanza parse failed; 1 - incorrect Partial DRS; 2 - incorrect final DRS; 3 - incorrect SPARQL query; 4 - correct answer)
* template-id = template identification assigned by DBLP-QuAD (https://huggingface.co/datasets/awalesushil/DBLP-QuAD)
* SPARQL = SPARQL query of the natural language question of DBLP-QuAD (https://huggingface.co/datasets/awalesushil/DBLP-QuAD)
