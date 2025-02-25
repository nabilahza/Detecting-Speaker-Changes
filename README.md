# Detecting-Speaker-Changes

This project focuses on Speaker Change Detection (SCD) using the IEMOCAP dataset, leveraging Fundamental Frequency (F0) and Mel-Frequency Cepstral Coefficients (MFCCs) as features. The primary goal is to classify speaker changes using a Long Short-Term Memory (LSTM) model with parameter tuning.

#### Dataset
IEMOCAP Dataset: Contains dialog sessions with labeled speaker changes.

#### Features extracted:
Fundamental Frequency (F0) (pitch-related feature)
MFCCs (captures spectral properties of speech)

##### Methodology
Feature Extraction:

Used a sliding window approach with two configurations:
- 20ms window, 10ms overlap
- 40ms window, 10ms overlap
Extracted features using Librosa/Praat-Parselmouth.

#### Data Preprocessing:

Assigned binary labels (1 for speaker change, 0 for no change).
Split data into train (sessions 1-3), validation (session 4), test (session 5).

#### Model Development:

Implemented an LSTM-based classifier for speaker change detection.
Performed parameter tuning for different window sizes.
Evaluated model using F1-score, precision, recall.

##### Results & Discussion:

Analyzed model performance across different window sizes.
Compared accuracy, strengths, and weaknesses of each configuration.
