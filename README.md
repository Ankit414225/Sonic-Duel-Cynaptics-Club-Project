# Sonic-Duel-Cynaptics-Club-Project
PS-1
This Project is a Deep CNN for environment sound classification,trained using MEI Spectogram,with Data Augmentation

_______________________________________________________________________________________________
_______________________________________________________________________________________________
Dataset Descrp:
Audio clips are converted into log-Mei spectograms

_______________________________________________________________________________________________
_______________________________________________________________________________________________

Key Features:
Advanced data augmentation:

1.Time stretching

2.Pitch shifting

3.Random noise injection

Deeper CNN architecture:
4 convolutional blocks (64 → 128 → 256 → 512 filters)


Automatic test prediction + Kaggle submission file

_________________________________________________________________________________________________
_________________________________________________________________________________________________
Model Architecture (DeepAudioCNN)
Convolution Blocks

Block 1: 64 filters × 2 conv layers

Block 2: 128 filters × 2 conv layers

Block 3: 256 filters × 2 conv layers

Block 4: 512 filters × 2 conv layers

Each block:

Conv → BN → ReLU → Conv → BN → ReLU → MaxPool → Dropout

Fully Connected Layers

Linear: 1024

Linear: 512

Linear: 256

Total parameters:15M+

________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________

Audio Feature Extraction

Each audio file is converted to a log-Mel spectrogram:

sr = 22050

duration = 2.5 seconds

n_mels = 128

____________________________________________________________________________________________________________________________________________________________________Model is trained using:

Adam optimizer

CrossEntropy loss

Early stopping with patience

