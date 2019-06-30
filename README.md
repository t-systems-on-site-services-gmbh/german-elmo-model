# German ELMo Model
This is a german [ELMo deep contextualized word representation](https://allennlp.org/elmo). It is trained on a special [German Wikipedia Text Corpus](https://github.com/t-systems-on-site-services-gmbh/german-wikipedia-text-corpus).

ELMo is a deep contextualized word representation that models both 
1. complex characteristics of word use (e.g., syntax and semantics)
2. how these uses vary across linguistic contexts (i.e., to model polysemy)

These word vectors are learned functions of the internal states of a deep bidirectional language model (biLM), which is pre-trained on a large text corpus. They can be easily added to existing models and significantly improve the state of the art across a broad range of challenging NLP problems, including question answering, textual entailment and sentiment analysis. More about these "Deep contextualized word representations" can be found here: https://arxiv.org/abs/1802.05365

This pretrained model can be used with [bilm-tf](https://github.com/allenai/bilm-tf) (the tensorflow implementation of ELMo). Before usage it can (should) be fine tuned with your domain specific data (see below).

## How this ELMo Model has been generated
[...]

## How to use this ELMo Model
[...]

## Content of the Tarball
These files are needed to use the ELMo model:
- vocab-train.txt - vocabulary file
- weights.hdf5 - weights from the trained biLM in hdf5 format
- options.json - options file which describes the hyperparameters of the biLM

These files are part of the tensorflow checkpoint mechanism. It can save and restore TensorFlow models. This is needed to do fine tuning (see below):
- checkpoint
- model.ckpt-5265680.index
- model.ckpt-5265680.meta
- model.ckpt-5265680.data-00000-of-00001

## Download
- [bilm-output-result.tgz.part-00]()
  - MD5: 755379908885a6fa6fb5b68e4806eae0
  - SHA1: 39b16d8eaeaa6ff8c161d092fd223704cc3963e6
- [bilm-output-result.tgz.part-01]()
  - MD5: 0a6544017c64cda91a2b209ecbdc5f2c
  - SHA1: 4647c43037b01a67e6c206c9748c5e5b8ab936f8
- [bilm-output-result.tgz.part-02]()
  - MD5: f316774e8bd12d078bd5e869c64be14b
  - SHA1: 10530cb852cf26f6340c2b4d1cfbeb882f44692b
- [bilm-output-result.tgz.part-03]()
  - MD5: ae44a2d3cf95795edacba690b77a4e7b
  - SHA1: c54bcdc27d769e2c5a077d7ab342ee34dd1f3ec2
- bilm-output-result.tgz
  - MD5: 2aa41bbc32d42eae052a7ddf37909443
  - SHA1: 9af7efbdd480a919c45e11188625d59a5943f9b9

[TODO: Add Links]

## Unpack
Using these commands you can unpack the files (Linux and macOS):
```
cat bilm-output-result.tgz.part-* > bilm-output-result.tgz
tar xvfz bilm-output-result.tgz
```
