# Coreference resolution

Coreference resolution is the task of clustering mentions in text that refer to the same underlying real world entities.

Example:

```
               +-----------+
               |           |
I voted for Obama because he was most aligned with my values", she said.
 |                                                 |            |
 +-------------------------------------------------+------------+
```

"I", "my", and "she" belong to the same cluster and "Obama" and "he" belong to the same cluster.

### CoNLL 2012

Experiments are conducted on the data of the [CoNLL-2012 shared task](http://www.aclweb.org/anthology/W12-4501), which
uses OntoNotes coreference annotations. Papers
report the precision, recall, and F1 of the MUC, B3, and CEAFφ4 metrics using the official
CoNLL-2012 evaluation scripts. The main evaluation metric is the average F1 of the three metrics.

| Model           | Avg F1 |  Paper / Source | Code |
| ------------- | :-----:| --- | --- |
| Joshi et al. (2019)<sup>[1](#myfootnote1)</sup> | 76.9 | [BERT for Coreference Resolution: Baselines and Analysis](https://arxiv.org/abs/1908.09091) | [Official](https://github.com/mandarjoshi90/coref) |
| Kantor and Globerson (2019) | 76.6 | [Coreference Resolution with Entity Equalization](https://www.aclweb.org/anthology/P19-1066/) | [Official](https://github.com/kkjawz/coref-ee) |
| Fei et al. (2019) | 73.8 | [End-to-end Deep Reinforcement Learning Based Coreference Resolution](https://www.aclweb.org/anthology/P19-1064/) | |
| (Lee et al., 2017)+ELMo (Peters et al., 2018)+coarse-to-fine & second-order inference (Lee et al., 2018) | 73.0 | [Higher-order Coreference Resolution with Coarse-to-fine Inference](http://aclweb.org/anthology/N18-2108) | [Official](https://github.com/kentonl/e2e-coref) |
| (Lee et al., 2017)+ELMo (Peters et al., 2018) | 70.4 | [Deep contextualized word representatIions](https://arxiv.org/abs/1802.05365) | |
| Lee et al. (2017) | 67.2 | [End-to-end Neural Coreference Resolution](https://arxiv.org/abs/1707.07045) | |


<a name="myfootnote1">[1]</a> Joshi et al. (2019): (Lee et al., 2017)+coarse-to-fine & second-order inference (Lee et al., 2018)+BERT (Devlin et al., 2019)


[Go back to the README](../README.md)
