# Face Super Resolution
The primary aim of the Face-Image Super Resolution (SR) is 
to construct the High Resolution (HR) face images from the 
Low Resolution (LR) face images. Existing techniques for 
Super Resolution mostly rely on either the prior facial 
knowledge, prior image degradation information for better 
HR results, but it often led to limited generalization over 
images from different sources. In recent years, state of the 
art techniques for Face Image SR using GANs were 
introduced, which produces promising results. Therefore, 
we thoroughly studied the different GANs-based 
techniques and found HiFaceGAN and ESRGAN approaches. 
We adopt different ideas from these models as baseline 
and implemented our own version with few enhancements 
. To bring novelty and to further enhanced the results, we 
proposed multiple improvements in the architecture of 
ESRGAN. We replaced the standard discriminator loss of 
ESRGAN with PatchGAN discriminator from pix2pix GAN to 
reduce the unrealistic effect of artifacts in the 
reconstructed images and used LPIPS loss on face datasets 
for 4x upscaling factor. With extensive experiments with 
different loss functions to get more realistic images, 
proposed model yields more realistic and enhanced results 
than the original ESRGAN model
## Folder Structure

The directory structure of the developed project is shown as follows.

```
Getty_Bert_Fine_Tune
│   README.md
│   requirements.txt
│
└───src
│   │
│   │   │
│   │   datasets.py
│   │    
│   │   │   │   preprocessing.py
│   │   │   │   test_data_generation.py
│   │   │   │   train_data_generation.py 
│   │   │ 
│   │   └───training
│   │   │   │  train.py
│   │   │

│   │   
└─── Checkpoints
│   │   .
│   │   
```

## How to Run

The code can be run by the following command in the bash or command line in the root dir.

```
python src\train.py
```



