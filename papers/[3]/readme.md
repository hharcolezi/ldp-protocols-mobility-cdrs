## Title
Differentially Private Multivariate Time Series Forecasting of Aggregated Human Mobility With Deep Learning: Input or Gradient Perturbation?

## Abstract
This paper investigates the problem of forecasting multivariate aggregated human mobility while preserving the privacy of the individuals concerned. Differential privacy, a state-of-the-art formal notion, has been used as the privacy guarantee in two different and independent steps when training deep learning models. On one hand, we considered *gradient perturbation*, which uses the differentially private stochastic gradient descent algorithm to guarantee the privacy of each time series sample in the learning stage. On the other hand, we considered *input perturbation*, which adds differential privacy guarantees in each sample of the series before applying any learning. We compared four state-of-the-art recurrent neural networks: Long Short-Term Memory, Gated Recurrent Unit, and their Bidirectional architectures, i.e., Bidirectional-LSTM and Bidirectional-GRU. Extensive experiments were conducted with a real-world multivariate mobility dataset, which we published openly along with this paper. As shown in the results, differentially private deep learning models trained under gradient or input perturbation achieve nearly the same performance as non-private deep learning models, with loss in performance varying between 0.57% to 2.8%. The contribution of this paper is significant for those involved in urban planning and decision-making, providing a solution to the human mobility multivariate forecast problem through differentially private deep learning models.

## Experiments
* Please refer to [1_BiGRU.ipynb](https://github.com/hharcolezi/ldp-protocols-mobility-cdrs/blob/main/papers/%5B3%5D/1_BiGRU.ipynb) for the experimental evaluation with non-private DL models.
* Please refer to [2_BiGRU[GP].ipynb](https://github.com/hharcolezi/ldp-protocols-mobility-cdrs/blob/main/papers/%5B3%5D/2_BiGRU%5BGP%5D.ipynb) for the experimental evaluation with differentially private DL models through gradient perturbation.
* Please refer to [3_BiGRU[IP].ipynb](https://github.com/hharcolezi/ldp-protocols-mobility-cdrs/blob/main/papers/%5B3%5D/3_BiGRU%5BIP%5D.ipynb) for the experimental evaluation with differentially private DL models through input perturbation.

## Dataset
The multivariate time series dataset we use for the experiments is available here as [ML_final_df_real.csv](https://github.com/hharcolezi/ldp-protocols-mobility-cdrs/blob/main/papers/%5B3%5D/ML_final_df_real.csv).

## Bibtex
If you consider using our findings and dataset in your research, we would appreciate a reference to:

```bash
@misc{Arcolezi2022,
  doi = {10.48550/ARXIV.2205.00436},
  url = {https://arxiv.org/abs/2205.00436},
  author = {Arcolezi,  Héber H. and Couchot,  Jean-Fran\c{c}ois and Renaud,  Denis and Bouna,  Bechara Al and Xiao,  Xiaokui},
  title = {Differentially Private Multivariate Time Series Forecasting of Aggregated Human Mobility With Deep Learning: Input or Gradient Perturbation?},
  publisher = {arXiv},
  year = {2022}
}
```

Please notice this bibtex entry will be updated with the accepted version that will be published in the [NCAA journal](https://www.springer.com/journal/521).
