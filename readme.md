This project is a very typical example of when not to use the exact dataset as it is provided. Rather one should focus on transforming it into 
useful features for data extraction. In this project audio files are given in the dataset and naively I rushed to use a neural network to 
classify the audio files, however after research it was found that the correct approach was to convert the audio files into spectrographs for
each audio file and then perform classification on the. Some key points observed are:-

1. The dataset is spreaded in wrong naming scheme making me use inefficient functions to extract it
2. The librosa library wasn't use to its full capability with respect to the problem.
3. Fourier trasnformation was used on the waves to make them easier to classify.
4. Neural network gives low accuracy because the audio waves are highly spread over a range and the dataset was too samll (80 samples).
5. The waves were padded with another wave to generate extra feature in classification.