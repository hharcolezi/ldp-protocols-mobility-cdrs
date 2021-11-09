## Title
Improving the Utility of Locally Differentially Private Protocols for Longitudinal and Multidimensional Frequency Estimates

## Abstract
This paper investigates the problem of collecting multidimensional data throughout time (i.e., longitudinal studies) for the fundamental task of frequency estimation under local differential privacy (LDP). Contrary to frequency estimation of a single attribute (the majority of the works), the multidimensional aspect imposes to pay particular attention to the privacy budget. Besides, when collecting user statistics longitudinally, privacy progressively degrades. Indeed, both "multiple" settings combined (i.e., many attributes and several collections throughout time) imposes several challenges, in which this paper proposes the first solution for frequency estimates under LDP. To tackle these issues, we extend the analysis of three state-of-the-art LDP protocols (Generalized Randomized Response - GRR, Optimized Unary Encoding - OUE, and Symmetric Unary Encoding - SUE) for both longitudinal and multidimensional data collections. While the known literature uses OUE and SUE for two rounds of sanitization (a.k.a. memoization), i.e., L-OUE and L-SUE, respectively, we analytically and experimentally show that starting with OUE and then with SUE provides higher data utility (i.e., L-OSUE). Also, for attributes with small domain sizes, we propose longitudinal GRR (L-GRR), which provides higher utility than the other protocols based on unary encoding. Lastly, we also propose a new solution named **A**daptive **L**DP for **LO**ngitudinal and **M**ultidimensional **FRE**quency **E**stimates (ALLOMFREE), which randomly samples a single attribute to send with the whole privacy budget and adaptively selects the optimal protocol, i.e., either L-GRR or L-OSUE. As shown in the results, ALLOMFREE consistently and considerably outperforms the state-of-the-art L-SUE and L-OUE protocols in the quality of the frequency estimations.

## Experiments
* Please refer to [1_ALLOMFREE_Analysis.ipynb](https://github.com/hharcolezi/ldp-protocols-mobility-cdrs/blob/main/papers/%5B4%5D/1_ALLOMFREE_Analysis.ipynb) for the theoretical analysis.

## Bibtex
@misc{arcolezi2021improving,
      title={Improving the Utility of Locally Differentially Private Protocols for Longitudinal and Multidimensional Frequency Estimates}, 
      author={Héber H. Arcolezi and Jean-François Couchot and Bechara Al Bouna and Xiaokui Xiao},
      year={2021},
      eprint={2111.04636},
      archivePrefix={arXiv},
      primaryClass={cs.CR}
}
