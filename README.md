Companion code for the accepted paper at NeurIPS'19 Workshop "Real Neurons & Hidden Units: Future directions at the intersection of neuroscience and artificial intelligence".

"Estimating encoding models of cortical auditory processing using naturalistic stimuli and transfer learning"

Our encoding models are trained on SoundNet features. We provided the SoundNet features, and also explain the method to regenerate them in step 1.

# CODE : 

## requirements 

-Python 3.7
-nilearn
-sklearn
-pandas
-matplotlib
-numpy
-scipy
-tqdm
-pytorch
-soundfile
-librosa


# 1 - to extract features from SoundNet : 
- download the stimulus from openneuro : https://openneuro.org/crn/datasets/ds001110/snapshots/00003/files/stimuli:Sherlock.m4v and convert it into a wave file at 22050 Hz. 
- Follow the instructions here https://github.com/smallflyingpig/SoundNet_Pytorch to download the sound8.pth
- run the notebook "1_ExtractSoundNetFeatures.ipynb"

# 2 - To estimate encoding models : 

Run the notebook "2_encoding_with_parcellation.ipynb"

Please read the instructions inside carefully, and configure the various path accordingly.

# DATA :

 We include R2 maps for encoding models estimated on conv7 layer, using 1000 neurons in the hidden layers. 
 ALl other maps can be regenerated using the provided code. 
