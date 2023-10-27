# GANs with Python

## Setup

### Running in Colab

Open the file in Google Colab. If using own data files, make sure they're in `.drive/MyDrive/gans-workshop-files/name-of-your-data-folder`.

### Running locally

This will need a GPU on your machine. Install either Conda or Mamba. Use the environment.yml to then create the environment.

## Usage

`do_preprocess` - Set to `True` if this is the first time you are running the GAN with your dataset, otherwise set to `False`.
`from_checkpoint` - Set to `True` if you wish to have the GAN use a model file that was created from a previous run, otherwise set to `False`.
`student_uploaded_own_data` - Set to `True` if you have your own data files that you want to use, otherwise set to `False` and it will download some images for you from the Oxford flower dataset.

## Descriptions

Keeping these here so I don't lose them.

### Longer Description

This workshop introduces students to the use of Generative Adversarial Networks (GANs) for creating synthetic images. In this hands-on session, participants will dive into the fundamentals of GANs using the TensorFlow library, learning to build and train their very own basic GAN model. Students will also be taught how and why GPUs are used to accelerate the training process. We'll also introduce you to essential Python libraries like NumPy and Matplotlib for data manipulation and visualisation, and guide you through the process of loading GANs models and analysing their performance.

### Shorter Description

This workshop builds on the introductory Python course and teaches students how to create synthetic images with Generative Adversarial Networks (GANs) using TensorFlow. Participants will build and train a basic GAN model and learn about GPU acceleration. We'll also cover key Python libraries like NumPy and Matplotlib for data manipulation and visualisation, along with loading GAN models and evaluating their performance.

