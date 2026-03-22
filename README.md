# DL-23f1001065-t12026
* Name : Akash Kumbhakar
* ID : 23f1001065
# A Kaggle competetion on Music genre classification using DeepLearning based models building.
# Overview : 
The Messy Mashup competition focuses on robust music genre classification under realistic and noisy mixing conditions. Participants are provided with a curated training dataset consisting of songs from 10 distinct music genres, where each song is instrument-separated into four stems: drums.wav, vocals.wav, bass.wav, and others.wav. In addition, a separate dataset containing random noise sounds is supplied.

The core challenge lies in generalization. Instead of clean, original tracks, the test data is composed of mashups created by mixing instrument stems from different songs belonging to the same genre. To ensure musical coherence during mixing, some instrument tracks may undergo tempo adjustments so that all stems are rhythmically synchronized before being combined. To further increase complexity and simulate real-world audio conditions, random noise samples are added to these mashups at varying intensities and positions.
# Repository Structure : 
                                  main branch                                                             milestone branches
                                      |                                                                           |
                                  /notebook                                                                       |
                                      |                                                                milestone wise notebooks
                                      |
    |---------------------------------|------------------------------------------|
    |                                 |                                          |
    /preprocessing                /training                                 /inference
                                      |
                                      |
                  |-------------------|--------------------------|
                  |                   |                          |
                  |                   |                          |
                scratch_model      pretrained_model          third_model


# Evaluation Metric : 
Submissions are evaluated using the Macro F1 Score across the 10 genre classes:

    Macro F1 computes the F1 score independently for each genre and then averages them.
    This metric treats all genres equally, making it well-suited for evaluating performance under potential class imbalance.

Higher macro F1 scores indicate better overall genre classification performance across all classes.
