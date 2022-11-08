# gansformer-reproducibility-challenge

> Project for Advance Topic in Machine Learning course @ USI 21/22.  
> See https://github.com/GiorgiaAuroraAdorni/gansformer-reproducibility-challenge, https://drive.google.com/drive/folders/1sqHD-X4mLOOkoT-xJvWGdPlwxb5et0kA?usp=sharing for datasets and https://drive.google.com/drive/folders/1ZFfO4HVINH-aDQbgLscJxNTqGLEIOMZv?usp=sharing for models.

### Contributors

**Giorgia Adorni** — giorgia.adorni@usi.ch [GiorgiaAuroraAdorni](https://github.com/GiorgiaAuroraAdorni)

**Felix Boelter** — felix.boelter@usi.ch [felixboelter](https://github.com/felixboelter)

**Stefano Carlo Lambertenghi** — stefano.carlo.lambertenghi@usi.ch [steflamb](https://github.com/steflamb)

### Prerequisites

- Python 3
- Tensorflow 1.X

### Installation

Clone our repository and install the requirements

```sh
$ git clone https://github.com/GiorgiaAuroraAdorni/gansformer-reproducibility-challenge
$ cd gansformer-reproducibility-challenge/src
$ pip install -r requirements.txt
```

#### Usage

For the usage, go to the `colab notebooks` directory: 
- Run `Reproducibility_model_trainer.ipynb` for training the models: Stylegan2, GANformers with Simplex and Duplex Attention and GANformers with Simplex and Duplex Attention (with vanilla StyleGAN2 discriminator).  
- Run `Reproducibility_result_visualizer.ipynb` for the visualisation phase: here you can select the model that you want to use and generate random images, perform a symple interpolation of the latent space or even perform style mixing starting from a chosen target image.

#### Results
Reproducibility results for the GANFormer/StyleGAN2 hybrid. All of the results are found in the [Report](https://github.com/felixboelter/gansformer-reproducibility-challenge/blob/main/report/main.pdf).
#### FID scores
&emsp;&emsp;&emsp;&emsp;
(1) FID scores for the cartoon dataset
&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp; 
(2) FID scores for the FFHQ dataset

![FID Score cartoon dataset](https://github.com/felixboelter/gansformer-reproducibility-challenge/blob/main/report/images/FIDscore-cartoonset.png) ![FID Score FFHQ dataset](https://github.com/felixboelter/gansformer-reproducibility-challenge/blob/main/report/images/FIDscore-ffhq.png)
#### Generated images for the StyleGAN2 baseline and all types of GANFormer
![Generated images for the StyleGAN2 baseline and all types of GANFormer](https://github.com/felixboelter/gansformer-reproducibility-challenge/blob/main/report/images/imgAll.png)

##### Latent space interpolation for GANFormer model with Duplex attention on the Generator
![Interpolation of images from the GANFormer with Duplex attention and a StyleGAN2 discriminator](https://github.com/felixboelter/gansformer-reproducibility-challenge/blob/main/report/images/interpolation_GANFormer_Duplex_D_Stylegan2_300kimg.png)

##### Latent space interpolation for GANFormer model with Simplex attention on the Generator
![Interpolation of images from the GANFormer with Simplex attention and a StyleGAN2 discriminator](https://github.com/felixboelter/gansformer-reproducibility-challenge/blob/main/report/images/interpolation_GANFormer_Simplex_D_Stylegan2_300kimg.png)
