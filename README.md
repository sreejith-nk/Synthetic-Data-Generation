# Synthetic-Data-Generation

The steps used are as follows,
- We used VAM Deep Learniing model for syntetic data generation.
- We then trained a lightGBM model on this bigger dataset to make the predictions.

## VAM
VAM (Variational Autoencoder with Adversarial Learning and Multi-Modality Fusion) is a deep learning model that is designed for multi-modal data generation and fusion tasks. It is based on a variational autoencoder (VAE) architecture, which is a type of generative model that learns to generate new samples from a given distribution.

The VAM model consists of three main components: a VAE, an adversarial learning module, and a multi-modal fusion module.

The VAE component of the model is responsible for learning the distribution of each modality (i.e., the probability distribution of the data) and generating new samples that are consistent with this distribution. The VAE is trained using a combination of a reconstruction loss, which measures the difference between the generated and actual data, and a KL divergence loss, which measures the difference between the learned distribution and a prior distribution.

The adversarial learning module of the VAM model consists of a discriminator network that is trained to distinguish between real and generated data. This module is added to improve the quality of the generated samples and make them more realistic. The generator (VAE) and discriminator networks are trained using a joint loss function that combines the reconstruction and adversarial losses.

The multi-modal fusion module of the VAM model is responsible for fusing the generated samples from each modality to create a new sample that combines the information from all modalities. This module uses a linear fusion approach to combine the generated samples and produce the final output.

One of the strengths of the VAM model is its ability to handle missing or incomplete data. The VAE component of the model is capable of generating new samples that are consistent with the distribution of the input data, even when parts of the data are missing or corrupted. This makes the VAM model useful for applications such as medical imaging, where missing data is common.

Overall, the VAM model is a powerful deep learning model that can generate high-quality multi-modal data and fuse information from different modalities to produce new samples. Its architecture is carefully designed to leverage the strengths of VAEs and adversarial learning for multi-modal data generation and fusion tasks.
