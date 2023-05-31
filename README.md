## Benchmarking Spectral Image Generation Schema and Pre-Trained Convolutional Neural Network Architectures for Audio Classification Tasks
 
## Abstract:

Recent advancements in image classification such as Convolutional Neural Networks can be employed to perform audio classification.  While there has been work done on benchmarking different networks and image representations, many techniques remain unexplored.  Three popular pre-trained image networks (EfficentNet-b0, ResNet50, SqueezeNet) and four different image representations of audio (Cochleagram, Approximate Cochleagram, Linear Gammachirp, and Logarithmic Gammachirp) are benchmarked by performance and preprocessing cost using the UrbanSound8K audio dataset, which contains common sounds that contribute to noise pollution in urban areas.  EfficientNet-b0 and ResNet50 achieved comparable performance for each of the four data representations and significantly outperformed SqueezeNet. The Linear Gammachirp and the Cochleagram provided for the highest classification accuracy, with the Linear Gammachirp slightly but not significantly outperforming Cochleagrams.  Findings were surprising because the logarithmic gammachirp filter is a much more computationally complex model of the cochlear inner ear than the other three, and yet it yielded the worst results.  Findings suggest that more complex cochlear models can achieve but do not guarantee better results out of the box, and that optimal tuning of parameters in each cochlear representation may yield improved results.  The limitations of current classification techniques and suggestions for further exploration of different data representations are discussed.

## Contents:

### Final Whitepaper: 
Benchmarking Spectral Image Generation Schema and Pre-Trained Convolutional Neural Network Architectures for Audio Classification Tasks  

### Final Presentation:
Powerpoint presentation used in final thesis defense

### Data:  
Metadata for the UrbanSound8k dataset.  Due to the size of the audio dataset, only the metadata is included.  The full dataset can be found here: https://urbansounddataset.weebly.com/urbansound8k.html

### Code:  
**Data Preprocessing** - Jupyter Notebook - Python code relating to the preprocessing of audio files into image data representations  
**Preprocessing Time Benchmarking** - Jupyter Notebook - Python code used to benchmark of spectral image generation techniques  
**EfficientNet 10 fold** - Jupyter Notebook - Python code implementation of EfficientNet along with the 10 fold validation training process  
**ResNet50 10 fold** - Jupyter Notebook - Python code implementation of ResNet50 along with the 10 fold validation training process
**SqueezeNet 10 fold** - Jupyter Notebook - Python code implementation of ResNet50 along with the 10 fold validation training process
**Unused Models** - Folder - Network solutions not used in final experiment (Wave2Vec, VGG16, Scratch PyTorch, Scratch Tensorflow)  

### Experimental Results:  
Trained models (1 per fold) and train/test performance reports for each benchmarked image representation (Cochleagram, Approximate Gammatone, Linear Gammachirp, Logarithmic Gammachirp) and CNN architecture (EfficientNet, ResNet50, SqueezeNet)  

