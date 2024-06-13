# DATA 452 Winter-Spring 2024
## Bioacoustics Team

### Sucheen Sundaram | sssundar@calpoly.edu
### Anagha Sikha | arsikha@calpoly.edu
### Sophia Chung | spchung@calpoly.edu

### Statistics Department

### Bailey College of Science and Mathematics

### California Polytechnic State University, San Luis Obispo, CA 93407




In the Winter of 2024, we implemented an ensemble method of the variational autoencoder. We developed two main notebooks, **vae.ipynb** and **vae_mel.ipynb**. The first notebook implements the variational autoencoder model on a regular spectrogram scale. However, the MEL notebook implemented MEL scaling. The two notebooks handle the entire data pipeline. They load in the data, preprocess it (MEL where necessary), and feed it into the model architecture. Lastly, they contain functions to calculate binary classification metrics.

In Spring 2024, we experimented with a convolutional neural network. Our work is contained in the **ConvertWavToSpec.ipynb** notebook. Like the variational autoencoder notebooks, they handle the entire data preprocessing pipeline.
