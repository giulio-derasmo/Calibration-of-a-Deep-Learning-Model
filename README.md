# Calibration of a Deep Learning Model

When doing classification is a commong misconception to interpret $f(x)_i$ as the probability of pattern x being class i. This is true only when $P(y=i \mid x) = f(x)_i$, hence we say the model its **calibrated**. 
In this project following [1](https://arxiv.org/abs/1706.04599), I will measure the calibration of my model and calibrate it using as loss function the Focal Loss. A conformal prediction is done at the end to have another measure of the calibration.


### Results

Below the Confidence histogram (left) and Reliability diagram (right) of the model before calibration:

<p float="left">
  <img src="/images/confidence_histogram_model_not_calibrated.jpg" width="250" />
  <img src="/images/reliability_diagram_before_calibration.jpg" width="250" /> 
</p>

Below the Confidence histogram (left) and Reliability diagram (right) of the model after calibration using Focal-Loss:

<p float="center">
  <img src="/images/calibrated model.jpg" width="500" />
</p>
  

### References

[1] Guo, C., Pleiss, G., Sun, Y. and Weinberger, K.Q., 2017. [On calibration of modern neural networks](https://arxiv.org/abs/1706.04599). In *ICML* (pp. 1321-1330). PMLR.

[2] Mukhoti, J., Kulharia, V., Sanyal, A., Golodetz, S., Torr, P. and Dokania, P., 2020. [Calibrating deep neural networks using focal loss](https://proceedings.neurips.cc/paper/2020/hash/aeb7b30ef1d024a76f21a1d40e30c302-Abstract.html). In *Advances in Neural Information Processing Systems*, 33, pp. 15288-15299.

[3] Angelopoulos, A.N. and Bates, S., 2021. [A gentle introduction to conformal prediction and distribution-free uncertainty quantification](https://arxiv.org/abs/2107.07511). *arXiv preprint arXiv:2107.07511*.



#
<p align="center">
    <img src="https://user-images.githubusercontent.com/50860347/147412786-183da6b0-990f-4016-9f2e-0719d8066f5b.png" style="width: 100%"/>
<p>
