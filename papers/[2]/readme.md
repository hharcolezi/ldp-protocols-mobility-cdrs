## Title
Random Sampling Plus Fake Data: Multidimensional Frequency Estimates With Local Differential Privacy

## Abstract
With local differential privacy (LDP), users can privatize their data and thus guarantee privacy properties before transmitting it to the server (a.k.a. the aggregator). One primary objective of LDP is frequency (or histogram) estimation, in which the aggregator estimates the number of users for each possible value. In practice, when a study with rich content on a population is desired, the interest is in the multiple attributes of the population, that is to say, in multidimensional data (d >= 2). However, contrary to the problem of frequency estimation of a single attribute (the majority of the works), the multidimensional aspect imposes to pay particular attention to the privacy budget. This one can indeed grow extremely quickly due to the composition theorem. To the authors' knowledge, two solutions seem to stand out for this task: 1) splitting the privacy budget for each attribute, i.e., send each value with ε/d-LDP (*Spl*), and 2) random sampling a single attribute and spend all the privacy budget to send it with ε-LDP (*Smp*). Although *Smp* adds additional sampling error, it has proven to provide higher data utility than the former *Spl* solution. However, we argue that aggregators (who are also seen as attackers) are aware of the sampled attribute and its LDP value, which is protected by a "less strict" exp(ε) probability bound (rather than exp(ε/d)). This way, we propose a solution named **R**andom **S**ampling plus **F**ake **D**ata (RS+FD), which allows creating *uncertainty* over the sampled attribute by generating fake data for each non-sampled attribute; RS+FD further benefits from amplification by sampling. We theoretically and experimentally validate our proposed solution on both synthetic and real-world datasets to show that RS+FD achieves nearly the same or better utility than the state-of-the-art *Smp* solution.

## Experiments
* Please refer to [1_RS+FD_Analysis.ipynb](https://github.com/hharcolezi/ldp-protocols-mobility-cdrs/blob/main/papers/%5B2%5D/1_RS%2BFD_Analysis.ipynb) for the theoretical analysis.
* Please refer to [2_RS+FD_LDP_Synthetic3_50k_d10.ipynb](https://github.com/hharcolezi/ldp-protocols-mobility-cdrs/blob/main/papers/%5B2%5D/2_RS%2BFD_LDP_Synthetic3_50k_d10.ipynb) for the experimental evaluation with a synthetic dataset.
* Please refer to [2_RS+FD_LDP_VHs.ipynb](https://github.com/hharcolezi/ldp-protocols-mobility-cdrs/blob/main/papers/%5B2%5D/2_RS%2BFD_LDP_VHs.ipynb) for the experimental evaluation with a real-world and open dataset.

## Recommended citation
```bash
Héber H. Arcolezi, Jean-François Couchot, Bechara Al Bouna, and Xiaokui Xiao. 2021. Random Sampling Plus Fake Data: Multidimensional Frequency Estimates With Local Differential Privacy. In Proceedings of the 30th ACM International Conference on Information and Knowledge Management (CIKM’21), November 1–5, 2021, Virtual Event, QLD, Australia. ACM, New York, NY,USA, 11 pages. https://doi.org/10.1145/3459637.3482467.
```

## Bibtex
```bash
@inproceedings{Arcolezi2021,
  doi = {10.1145/3459637.3482467},
  url = { https://doi.org/10.1145/3459637.3482467 },
  year = {2021},
  month = nov,
  publisher = {ACM},
  author = {Héber H. Arcolezi and Jean-François Couchot and Bechara Al Bouna and Xiaokui Xiao},
  title = {Random Sampling Plus Fake Data: Multidimensional Frequency Estimates With Local Differential Privacy},
  booktitle = {Proceedings of the 30th ACM International Conference on Information \& Knowledge Management}
}
```
