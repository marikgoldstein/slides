Some work in progress slides on diffusions from a variational perspective.

Mixture of gaussian to VAE to a latent variable model with tons of latent variables, each the same shape as the data, which leads to a diffusion model.

Score matching loss doesn't pop out of nowhere, but instead, is what you get when you derive the elbo for this latent variable model and then apply Stein's Lemma. Then the usual diffusion losses are just that elbo with some constants and scalings dropped.

These were mostly meant to have a spoken-along lecture but I'll try to edit them to be standalone.

References. A few of the images in the above slides come from

- [CVPR Diffusion Tutorial](https://cvpr2023-tutorial-diffusion-models.github.io/)
- [Yang Song's various slides](https://yang-song.net/blog/2021/score/)
- [https://stability.ai/](https://stability.ai/)
- [https://restofworld.org/2023/ai-image-stereotypes/](https://restofworld.org/2023/ai-image-stereotypes/)

A few of the equations/plots come from 

- [Kingma and Welling, VAE](https://arxiv.org/abs/1312.6114)
- [Sohl-Dickstein et al, Deep Unsupervised Learning using Nonequilibrium Thermodynamics](https://arxiv.org/abs/1503.03585)
- [Ho et al, DDPMs](https://arxiv.org/abs/2006.11239)
- [Dockhorn et al, Crtically-Damped Langevin](https://arxiv.org/abs/2112.07068)
- [Huang et al, variational perspective on diffusions](https://arxiv.org/abs/2106.02808)

The variational perspective is there right in Sohl-Dickstein 2015 and Ho 2020. Then in 2021, Huang, Kingma, Song, and others show that the continuous time objective can yield an elbo too.

A few more images come from soon to be posted work with collaborators and will be credited here soon.



