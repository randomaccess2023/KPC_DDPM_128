# Denoising Diffusion Probabilistic Model for Generating Histopathology Images

The source code for the conference paper designated _**Denoising Diffusion Probabilistic Model for generating Histopathology Images**_ has been shared in this GitHub repository.

I will explain different _**folders**_ and _**files**_ available in this repository concisely to make things easy for the users.

- ### Let's focus on the `P1` folder first:
1. `Part1_KPC_DDPM_Linear_Training.ipynb`: This file hosts the code for training the unconditional DDPM using a `linear` variance scheduler.
2. `Part2_KPC_DDPM_Linear_Sampling.ipynb`: This file features the code to randomly generate histopathology samples using the trained unconditional DDPM via a `linear` variance scheduler.
3. `Part3_KPC_DDPM_Linear_FID.ipynb`: This file provides the implementation for calculating the FID distance using the original images and the images generated with a trained unconditional DDPM using a `linear` variance scheduler.
4. `Part4_KPC_DDPM_Linear_Forward_Process.ipynb`: This file features the code to obtain results following the forward process using a `linear` variance scheduler.
5. `__init__.py`: This is an empty file which is required to mark a directory as a Python package.
6. `hist_ddpm_20240507.150.tsv`: This file contains the the unconditional DDPM training metrics using a `linear` variance scheduler.

- ### Now, let's focus on the `P2` folder:
1. `Part1_KPC_DDPM_Cosine_Training.ipynb`: This file hosts the code for training the unconditional DDPM using a `cosine` variance scheduler.
2. `Part2_KPC_DDPM_Cosine_Sampling.ipynb`: This file features the code to randomly generate histopathology samples using the trained unconditional DDPM via a `cosine` variance scheduler.
3. `Part3_KPC_DDPM_Cosine_FID.ipynb`: This file provides the implementation for calculating the FID distance using the original images and the images generated with a trained unconditional DDPM using a `cosine` variance scheduler.
4. `Part4_KPC_DDPM_Cosine_Forward_Process.ipynb`: This file features the code to obtain results following the forward process using a `cosine` variance scheduler.
5. `__init__.py`: This is an empty file which is required to mark a directory as a Python package.
6. `hist_ddpm_20240508.150.tsv`: This file contains the the unconditional DDPM training metrics using a `cosine` variance scheduler.

- ### Next, we focus on the `P3` folder:
1. `Part1_KPC_DDPM_Sigmoid_Training.ipynb`: This file hosts the code for training the unconditional DDPM using a `sigmoid` variance scheduler.
2. `Part2_KPC_DDPM_Sigmoid_Sampling.ipynb`: This file features the code to randomly generate histopathology samples using the trained unconditional DDPM via a `sigmoid` variance scheduler.
3. `Part3_KPC_DDPM_Sigmoid_FID.ipynb`: This file provides the implementation for calculating the FID distance using the original images and the images generated with a trained unconditional DDPM using a `sigmoid` variance scheduler.
4. `Part4_KPC_DDPM_Sigmoid_Forward_Process.ipynb`: This file features the code to obtain results following the forward process using a `sigmoid` variance scheduler.
5. `__init__.py`: This is an empty file which is required to mark a directory as a Python package.
6. `hist_ddpm_20240509.150.tsv`: This file contains the the unconditional DDPM training metrics using a `sigmoid` variance scheduler.

- ### The folder `Figures` has 5 folders inside it: `Figure 1`, `Figure 2`, `Figure 3`, `Figure 4`, and `Figure 5`. These 5 folders have the figures that can be seen in the conference paper.

- ### The folder `MODULES` has three `.py` files: `ATTEND.py`, `DENOISING_DIFFUSION_PYTORCH.py`, and `__init__.py`. `ATTEND.py` stores some helper functions. `DENOISING_DIFFUSION_PYTORCH.py` offers the building blocks required to construct the DDPM architecture. `__init__.py` is an empty file.

Finally, `inception_score.ipynb` shows the code for calculating the inception score using images geenrated with all the schedulers (`linear`, `cosine`, and `sigmoid`).

>> We haven't been able to provide the following things:

1. `model_ddpm_20240507.150.ckpt`: The model checkpoint for the unconditional DDPM trained with a `linear` variance scheduler.
2. `model_ddpm_20240508.150.ckpt`: The model checkpoint for the unconditional DDPM trained with a `cosine` variance scheduler.
3. `model_ddpm_20240509.150.ckpt`: The model checkpoint for the unconditional DDPM trained with a `sigmoid` variance scheduler.
4. `ORG`: The directory that contains 11,000 original images required for computing FID distance and inception score.
5. `GEN_Linear`: The directory that contains 11,000 generated images obtained using a `linear` variance scheduler and required for computing FID distance and inception score.
6. `GEN_Cosine`: The directory that contains 11,000 generated images obtained using a `cosine` variance scheduler and required for computing FID distance and inception score.
7. `GEN_Sigmoid`: The directory that contains 11,000 generated images obtained using a `sigmoid` variance scheduler and required for computing FID distance and inception score.

>> These 7 _files_ and _directories_ are too big and can't be shared in GitHub due to the limitations it has.

## This repository uses MIT License. Read the terms and conditions from _LICENSE_ text file.

> The conference paper is not available on the Internet yet. Once it is, we will provide the link for the readers to access it.
