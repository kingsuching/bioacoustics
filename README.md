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

To future teams working on the project:

You only need to run the **vae.ipynb** and **vae_mel.ipynb** notebooks. The pre-postprocessing notebooks contain all the functions necessary to clean the data and train the model.

Lastly, you must create an AWS S3 account to access the data stored in the whale-recordings bucket and get the files in the bucket. There is a pipeline that takes in a CSV file with your access key and secret key. That will return an S3 client object that will fetch all the data to your computer.

Disclaimer: The working directory structure may not be correct. Please modify it as necessary.
