![](https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=Python&logoColor=FFFFFF)
![](https://img.shields.io/badge/-Pytorch-EE4C2C?style=flat-square&logo=Pytorch&logoColor=FFFFFF)
![](https://img.shields.io/badge/-GoogleColab-F9AB00?style=flat-square&logo=GoogleColab&logoColor=FFFFFF)

# Diffusion Model Feast
This repository mostly provides a detailed description of the diffusion model (including code explanations, paper readings, etc.).
Most of the materials are from Hugging Face Diffusion Models Course(https://github.com/huggingface/diffusion-models-class)

Now, let's dive into it!

👩‍🎓Unit 1: An Introduction to Diffusion Models

There are two parts to this unit, namely Introduction to Diffusers and Diffusion Models from Scratch.

🧨In Introduction to Diffusers, I show the different steps described above using building blocks from the diffusers library. You'll quickly see how to create, train, and sample your own diffusion models on whatever data you choose. By the end of the notebook, you'll be able to read and modify the example training script to train diffusion models and share them with the world! This notebook also introduces the main exercise associated with this unit, where I will collectively attempt to figure out good 'training recipes' for diffusion models at different scales. See the next section for more info.

🤗Here is my code explanation: https://colab.research.google.com/drive/19APZrmXaIfSsfiz2Oxdx42VBmLKjTxsj?usp=sharing

🧑‍🔬In Diffusion Models from Scratch, I show those same steps (adding noise to data, creating a model, training and sampling) but implemented from scratch in PyTorch as simply as possible. Then I compare this 'toy example' with the diffusers version, noting how the two differ and where improvements have been made. The goal here is to gain familiarity with the different components and the design decisions that go into them so that when you look at a new implementation you can quickly identify the key ideas.

\:art\:Understaning the core API of Diffusers:
https://colab.research.google.com/github/huggingface/notebooks/blob/main/diffusers/diffusers_intro.ipynb#scrollTo=QQXXMLKkCbUJ

Three components consist of the core of API of Diffusers:

Pipelines: high-level classes designed to rapidly generate samples from popular trained diffusion models in a user-friendly fashion.

Models: popular architectures for training new diffusion models, e.g. UNet.

Schedulers: various techniques for generating images from noise during inference as well as to generate noisy images for training.

**!Two important things:**

schedulers are **parameter-free (no trainable weights)**

schedulers define the algorithm computing the slightly less noisy sample during inference

# Some Additional Resources

🏋️‍♂️AI Coffee Break video on Diffusion Models: https://www.youtube.com/watch?v=344w5h24-h8

🏋️‍♂️Lil’Log about Diffusion Models: https://lilianweng.github.io/posts/2021-07-11-diffusion-models/

🗺 Hungyi Lee's video on Diffusion Models: https://www.youtube.com/watch?v=azBugJzmz-o

🤗 Some Awesome Diffusion Models: https://github.com/diff-usion/Awesome-Diffusion-Models

Found more great resources? Let me know and I'll add them to this list.
