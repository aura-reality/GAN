# Neural Networks 
## Getting Started
- Video series (watch all the videos): https://www.youtube.com/watch?v=aircAruvnKk
- Neural Network Online Textbook: http://neuralnetworksanddeeplearning.com/index.html
- Guides: (http://ml4a.github.io/guides/) 
  - Classification: https://github.com/ml4a/ml4a-guides/blob/master/notebooks/keras_classification.ipynb
  - Convolutional: http://ml4a.github.io/ml4a/convnets/
  - Transfer Learning: https://github.com/ml4a/ml4a-guides/blob/master/notebooks/transfer-learning.ipynb
  - Recurrent: https://github.com/ml4a/ml4a-guides/blob/master/notebooks/recurrent_neural_networks.ipynb- 
 OpenAI overview of generative models: https://blog.openai.com/generative-models/
  
## GANs
- The paper that introduced GANs, but don't really need to read it: https://arxiv.org/abs/1406.2661
- GAN demo: https://github.com/Zackory/Keras-MNIST-GAN
- Tips and Tricks on Training GAN: https://github.com/soumith/ganhacks
- GAN Survey paper:  https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8195348

### VAE
- Trains a VAE using some simple feedforward nets to discriminate if the outputs look good: https://arxiv.org/pdf/1602.03220.pdf
- Mix a VAE with a GAN to get better loss instead of just L1 / L2 pixel loss https://arxiv.org/pdf/1512.09300.pdf
- Introspective Adversarial Network, a novel hybridization of the VAE and GAN https://arxiv.org/abs/1609.07093 

### Conditional Gans
- The paper that introduced *conditional* GANs: https://arxiv.org/pdf/1411.1784.pdf
- Isola Pixs2pixs paper (conditioning on an image - image to image translation): https://arxiv.org/pdf/1611.07004.pdf. Great blog post explaining the paper: https://affinelayer.com/pix2pix/
- Minor improvement on pix2pixs that gives each segmentation instance, allowing control by changing the input segmentation: https://tcwang0509.github.io/pix2pixHD/

### GAN manipulation: 
- Zhu et al. Explores the latent space using the inverse function: https://arxiv.org/pdf/1609.03552.pdf
- GAN Dissection, look at the sublayers in the gan to control outputs: https://arxiv.org/pdf/1811.10597.pdf
- How to interpolate in the latent space  https://openreview.net/pdf?id=BJslDBkwG
- How to interpolate the latent space tricks: https://arxiv.org/pdf/1609.04468.pdf
- BiGan - bidirectional gan - ie, latent to image, image to latent: https://arxiv.org/pdf/1605.09782.pdf
- Face editing: https://arxiv.org/pdf/1711.10678.pdf, https://github.com/LynnHo/AttGAN-Tensorflow/


### FiLM: 
Using linear modulation on feature layers (to encode conditional information or latent info). This is the inpsiration for the adaIN layers in the styleGAN paper. 
- Understand the basic idea: https://distill.pub/2018/feature-wise-transformations/
- SELF-MODULATION FOR GENERATIVE ADVERSARIAL NETWORKS Chen et al. https://arxiv.org/pdf/1810.01365.pdf. This encodes the latent as linear parameters later in the generator
- Using linear modulation for encoding conditional information: https://arxiv.org/pdf/1802.05637.pdf. (Seems like we can play off this one? How could a semantic segmentation be mapped to affine parameters to inject into a GAN?) 

### GAN state of the art : 
- NVIDIA "style transfer": https://arxiv.org/pdf/1812.04948.pdf
  * explainer blog post: https://towardsdatascience.com/explained-a-style-based-generator-architecture-for-gans-generating-and-tuning-realistic-6cb2be0f431
- ProGAN an earlier paper by the "style transfer" guys on improving resolution with multiple generators at increasing resolution:
  * https://arxiv.org/pdf/1710.10196.pdf
  * explainer blog: https://towardsdatascience.com/progan-how-nvidia-generated-images-of-unprecedented-quality-51c98ec2cbd2
  * released code: https://github.com/tkarras/progressive_growing_of_gans
- BigGAN, Google going nuts on training: https://arxiv.org/abs/1809.11096
- Vid2Vid: https://github.com/NVIDIA/vid2vid

### Image Compositing and other visual effects
- Deep Image Harmonization: https://arxiv.org/pdf/1703.00069.pdf
- ST-GAN: https://arxiv.org/pdf/1803.01837.pdf
- VFX.AI: list of tools/papers for visual effects with AI https://vfx.ai/
- Understanding asthetics: https://devblogs.nvidia.com/understanding-aesthetics-deep-learning/
- Deep Image Matting: https://arxiv.org/pdf/1703.03872.pdf 
- Compositing: https://arxiv.org/pdf/1807.07560.pdf
- LayoutGAN: generating layouts: https://openreview.net/forum?id=HJxB5sRcFQ


### Convolutional Generation
- DCGan, introduced convolutional Gan paper- https://github.com/Newmu/dcgan_code 
- Generating with a convolutional feedforward network with a regular loss function (ie, not a GAN): https://arxiv.org/pdf/1707.09405.pdf

### Other

- Deep Feature interpolation: https://arxiv.org/pdf/1611.05507.pdf
- Generating music: http://papers.nips.cc/paper/8023-the-challenge-of-realistic-music-generation-modelling-raw-audio-at-scale.pdf
- Using GANs to generate training data:  https://machinelearning.apple.com/2017/07/07/GAN.html
- GAN paper that combines multiple learned outputs into one final output (trained on only synthetic data!!!): https://arxiv.org/pdf/1703.10131.pdf 

### Training GANs
- Practical Recommendations for Gradient-Based Training of Deep Architectures https://arxiv.org/pdf/1206.5533v2.pdf
- Improved Techniques for Training GANs https://arxiv.org/pdf/1606.03498.pdf
- GAN Training Tips and Tricks: https://github.com/soumith/ganhacks
