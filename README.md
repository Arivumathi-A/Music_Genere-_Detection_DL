# Music Genre Classification
  The main goal of this music genre classification model using deep learning is to 
teach a computer to recognize different types of music. By training the model on a 
variety of songs from different genres, we want it to become really good at figuring 
out whether a song is pop, rock, jazz, or another genre. The idea is to make the model 
accurate, quick, and able to work well with any kind of music. This way, it can help 
organize music collections, recommend songs based on what you like, and even create 
playlists that match your mood. Ultimately, we want this model to be useful for music 
lovers, industry professionals, and researchers, making it easier for everyone to enjoy 
and explore the world of music.

# Challenges in the System
Limited and Inconsistent Dataset:
  Obtaining a comprehensive and diverse dataset covering various music genres can be 
challenging. The availability of labeled data may be limited, leading to difficulties 
in training models with sufficient examples of each genre. Moreover, inconsistencies 
in labeling or subjective categorization of genres across different sources can affect 
the dataset quality and model performance.

Imbalanced Representation:
  Similar to other classification tasks, there might be an imbalance in the number of 
audio samples among different genres. Some genres might have significantly more data 
compared to others, causing models to favor dominant genres and perform poorly on 
underrepresented ones.

Genre Ambiguity and Subjectivity:
  The categorization of music genres can be subjective and ambiguous. Genres might have overlapping 
characteristics or evolve over time, making it challenging to define clear boundaries between them. 
This subjectivity can introduce confusion in labeling and affect the model's ability to differentiate 
between closely related genres.

Generalization Across Diverse Audio Sources:
  Models trained on specific music genres or from particular audio sources might struggle to 
generalize well to new, unseen data. Variability in recording quality, musical styles, instruments 
used, and recording environments across different sources can pose challenges for models in accurately 
classifying genres outside their training domain.

Noise and Background Interference:
  Real-world audio data often contains background noise, overlapping sounds, or mixed genres, 
which can significantly impact classification accuracy. Handling noise robustly and distinguishing 
between actual genre characteristics and noise interference is a continual challenge in music genre 
classification.

Incorporating Temporal and Contextual Information:
  Capturing the temporal context and understanding the sequence of musical elements or patterns 
within a song can greatly enhance genre classification. However, effectively incorporating this temporal 
information while maintaining computational efficiency remains a challenge.

# Dataset Description
  The GTZAN dataset is the most-used public dataset for evaluation in machine listening research for 
  music genre recognition (MGR). The files were collected in 2000-2001 from a variety of sources including 
  personal CDs, radio, microphone recordings, in order to represent a variety of recording conditions
A collection of 10 genres with 100 audio files each, all having a length of 30 seconds. Blues, Classical, 
Country, Disco, Hip-hop, Jazz, Metal, Pop, Reggae, and Rock are among the ten music genres represented in 
the dataset. A visual representation for each audio file. One way to classify data is through neural networks. 
Because CNNs usually take in some sort of image representation, the audio files were converted to Mel Spectrograms 
to make this possible. Two csv files c ontaining features of the audio files. One file has for each 
song (30 seconds long) a mean and variance computed over multiple features that can be extracted from an 
audio file. The other file has the same structure, but the songs were split before into 3 seconds audio files 
(this way increasing 10 times the amount of data we fuel into our classification models). With data, more is 
always better.
Dataset link is https://www.kaggle.com/datasets/andradaolteanu/gtzan-dataset-music-genre-classification/data
