# DupGAN
PyTorch Implementation of <a href="">DupGAN</a> for Unsupervised Domain Adaptation(CVPR2018).
This code is implemented according to <a href="https://github.com/yunjey/mnist-svhn-transfer">CycleGAN</a>
## Prerequites
* [Python 3.5](https://www.continuum.io/downloads)
* [PyTorch 0.1.12](http://pytorch.org/)
## Train the model
```bash
$ python main.py --l2_reconst_loss=True
```
## Results in paper
* with different network architectures
** 1) Architectures in original paper of DupGAN
** 2) Architectures in DRCN: <a href="https://arxiv.org/abs/1607.03516">Deep Reconstruction-Classification Networks for Unsupervised Domain Adaptation</a>
<table>
  <tr>
    <th width=20%, bgcolor=yellow>Encoder architecture</th>
    <th width=20%, bgcolor=yellow>MNIST->USPS</th>
    <th width=20%, bgcolor=yellow>USPS->MNIST</th>
	<th width=20%, bgcolor=yellow>SVHN->MNIST</th>
	<th width=20%, bgcolor=yellow>MNIST->SVHN</th>
  </tr>
  <tr>
    <td bgcolor=#eeeeee> DRCN  </td>
    <td> 95.62</td>
	  <td> 94.67</td>
	  <td> 91.34</td>
	  <td> 60.26</td>
  </tr>
  <tr>
    <td bgcolor=#00FF00> OURS </td>
    <td> 96.01</td>
	  <td> 98.75</td>
	  <td> 92.46</td>
	  <td> 62.65</td>
  </tr>
</table>
