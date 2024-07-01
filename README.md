# DATA 452 Winter-Spring 2024
## Bioacoustics Team

### Sucheen Sundaram | sssundar@calpoly.edu
### Anagha Sikha | arsikha@calpoly.edu
### Sophia Chung | spchung@calpoly.edu

Statistics Department

Bailey College of Science and Mathematics

California Polytechnic State University, San Luis Obispo, CA 93407


----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

In the Winter of 2024, we implemented an ensemble method of the variational autoencoder, which can be found in the **VAE** folder. We developed two main notebooks, **vae.ipynb** and **vae_mel.ipynb**. The first notebook implements the variational autoencoder model on a regular spectrogram scale. However, the MEL notebook implemented MEL scaling. The two notebooks handle the entire data pipeline. They load in the data, preprocess it (MEL where necessary), and feed it into the model architecture. Lastly, they contain functions to calculate binary classification metrics.

In Spring 2024, we experimented with using a convolutional neural network and an object detection method. For the CNN, we looked at past team's work in the AWS notebooks and started to edit the **ConvertWavToSpec.ipynb** notebook to take in the Cal Poly Pier data. Like the variational autoencoder notebooks, they handle the entire data preprocessing pipeline. We were not able to edit the remaining notebooks in the pipeline **Develop&Train.ipynb** and **ModelEvaluation.ipynb**. All this work can be found in the **CNN** folder. For the object detection method, we followed a hugging face tutorial, and the notebook used is found in the **HuggingFace** folder.

To find any summaries and details of the processes we followed and past work we looked at, look in to the files in the **Documents** folder.

To future teams working on the project:

You only need to run the **vae.ipynb** and **vae_mel.ipynb** notebooks. The pre-postprocessing notebooks contain all the functions necessary to clean the data and train the model.

Lastly, you must create an AWS S3 account to access the data stored in the whale-recordings bucket and get the files in the bucket. There is a pipeline that takes in a CSV file with your access key and secret key. That will return an S3 client object that will fetch all the data to your computer.

Disclaimer: The working directory structure may not be correct. Please modify it as necessary.
