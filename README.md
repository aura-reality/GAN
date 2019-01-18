# Neural Networks 
## Getting Started
- Video series (watch all the videos): https://www.youtube.com/watch?v=aircAruvnKk
- Neural Network Online Textbook: http://neuralnetworksanddeeplearning.com/index.html
- Guides: (http://ml4a.github.io/guides/) 
  - Classification: https://github.com/ml4a/ml4a-guides/blob/master/notebooks/keras_classification.ipynb
  - Convolutional: http://ml4a.github.io/ml4a/convnets/
  - Transfer Learning: https://github.com/ml4a/ml4a-guides/blob/master/notebooks/transfer-learning.ipynb
  - Recurrent: https://github.com/ml4a/ml4a-guides/blob/master/notebooks/recurrent_neural_networks.ipynb
  
## GANs
- The paper that introduced GANs: https://arxiv.org/abs/1406.2661
- GAN demo: https://github.com/Zackory/Keras-MNIST-GAN
- Tips and Tricks on Training GAN: https://github.com/soumith/ganhacks
- GAN Survey paper:  https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8195348

### Conditional Gans
- The paper that introduced conditional GANs: https://arxiv.org/pdf/1411.1784.pdf
- Pics2pics paper (conditioning on an image/segmentation): https://arxiv.org/pdf/1611.07004.pdf
- The pic2pics competitor that gives each segmentation instance, allowing control by changing the input segmentation: https://tcwang0509.github.io/pix2pixHD/

### GAN manipulation: 
- Explores the latent space using the inverse function: https://arxiv.org/pdf/1609.03552.pdf
- GAN Dissection, look at the sublayers in the gan to control outputs: https://arxiv.org/pdf/1811.10597.pdf
- Another latent space exploration: https://openreview.net/pdf?id=BJslDBkwG
- haven't read it: https://arxiv.org/abs/1609.07093 
- interpolating the latent space tricks: https://arxiv.org/pdf/1609.04468.pdf

- https://arxiv.org/pdf/1611.05507.pdf

### GAN state of the art : 
- NVIDIA "style transfer": https://arxiv.org/pdf/1812.04948.pdf and https://arxiv.org/pdf/1810.01365.pdf, and an blog post: https://towardsdatascience.com/explained-a-style-based-generator-architecture-for-gans-generating-and-tuning-realistic-6cb2be0f431
- ProGAN an earlier paper by the "style transfer" guys on improving resolution with multiple generators at increasing resolution: https://arxiv.org/pdf/1710.10196.pdf
- BigGAN, Google going nuts on training: https://arxiv.org/abs/1809.11096

### Other
- Generating music: http://papers.nips.cc/paper/8023-the-challenge-of-realistic-music-generation-modelling-raw-audio-at-scale.pdf
- Using GANs to generate training data:  https://machinelearning.apple.com/2017/07/07/GAN.html
- GAN paper that combines multiple learned outputs into one final output (also trained on only synthetic data): https://arxiv.org/pdf/1703.10131.pdf 
