# SemBERT: Semantics-aware BERT for Language Understanding

**(2020/06/20) Update: Tips for possible issues**

"SRL prediction mismatches the provided samples"

The POS tags are slightly different using different spaCy versions.  SemBERT used spacy==2.0.18 to obtain the verbs.

Refer to [allenai/allennlp#3418](https://github.com/allenai/allennlp/issues/3418),  [cooelf/SemBERT#12](https://github.com/cooelf/SemBERT/issues/12) (CHN).

=========================================

Codes for the paper **[Semantics-aware BERT for Language Understanding](https://www.researchgate.net/publication/339301633_Semantics-aware_BERT_for_Language_Understanding)** in AAAI 2020

### **Overview**



## Requirements

(Our experiment environment for reference)

Python 3.6+
PyTorch (1.0.0)
AllenNLP (0.8.1)

## Datasets
GLUE data can be downloaded from [GLUE data](https://gluebenchmark.com/tasks) by running [this script](https://gist.github.com/W4ngatang/60c2bdb54d156a41194446737ce03e2e) and unpack it to directory <u>glue_data</u>.
We provide an example data sample in <u>glue_data/MNLI</u> to show how SemBERT works.

## Instructions
This repo shows the example implementation of SemBERT for NLU tasks.
We basically used the pre-trained BERT uncased models so do not forget to pass the parameter `--do_lower_case`.

The example script are as follows:


