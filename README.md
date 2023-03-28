# Benchmarking Spectral Image Generation Schema and Pre-Trained Convolutional Neural Network Architectures for Audio Classification Tasks
 
Recent advancements in image classification such as Convolutional Neural Networks can be employed to perform audio classification.  However, there are many ways audio data can be represented in image format, many hyperparameters that require tuning, and many networks that can be chosen for a selected task.  While there has been some work done on benchmarking these different networks and data representations, there are many techniques that remain unexplored.  There are also many considerations that have yet to be made regarding the consequences of preprocessing audio data into images – perhaps most notably, converting audio to a spectral image representation is an irreversible process.  In this research, three popular pre-trained image networks (EfficentNet-b0, ResNet50, SqueezeNet) of varying complexity and four different image representations of audio (Cochleagram, Approximate Cochleagram, Linear Gammachirp, and Logarithmic Gammachirp) are benchmarked by performance and preprocessing cost, using the UrbanSound8K audio dataset to classify sounds that are considered the main culprits of noise pollution in urban areas.  EfficientNet-b0 and ResNet50 achieved comparable performance for each of the four data representations and significantly outperformed SqueezeNet. The Linear Gammachirp and the Cochleagram provided for the highest classification accuracy of all the representations, with the Linear Gammachirp slightly but not significantly outperforming Cochleagrams.  Findings were surprising because the logarithmic gammachirp filter is a much more computationally complex model of the cochlear inner ear than the other three, and yet it yielded the worst results.  Findings suggest that more complex cochlear models can achieve but do not guarantee better results out of the box, and that optimal tuning of parameters in each cochlear representation may yield improved results.  The iterative nature of these tasks is discussed, along with the limitations of current classification techniques and suggestions for further exploration of different data representations.

