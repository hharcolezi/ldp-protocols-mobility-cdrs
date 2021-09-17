## Title
Differentially Private Multivariate Time Series Forecasting of Aggregated Human Mobility With Deep Learning: Input or Gradient Perturbation?

## Abstract
This paper investigates the problem of forecasting multivariate aggregated human mobility while preserving the privacy of the individuals concerned. Differential privacy (DP), a state-of-the-art formal notion, has been used as the privacy guarantee in two different and independent steps when training deep learning (DL) models. On the one hand, we considered *gradient perturbation*, which uses the differentially private stochastic gradient descent algorithm to guarantee the privacy of each time series sample in the learning stage. On the other hand, we considered *input perturbation*, which adds DP guarantees in each data sample of the series before applying any learning. To the authors' knowledge, this is the first work that evaluates differentially private DL models in both input and gradient perturbation settings on forecasting multivariate time series data. Experiments were carried out with a real-world mobility dataset from 2020 of 6 coarse regions in Paris, provided by Orange, a mobile network operator in France. As shown in the results, DL models trained under gradient or input perturbation achieve nearly the same performance as non-private DL models, with loss in performance varying between 0.57% -- 2.8%. Lastly, along with our results, we also published the mobility dataset in a Github repository such that other classical time series forecasting, machine learning, and privacy-preserving machine learning techniques can be tested and compared.

## Experiments
Currently cleaning the codes.

## Dataset
The multivariate time series dataset we use for the experiments is available here as [df_real.csv](https://github.com/hharcolezi/ldp-protocols-mobility-cdrs/blob/main/papers/%5B3%5D/df_real.csv).
