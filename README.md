# EEG-Signals-Classification

EEG signal classification is used to predict the right or left-hand movement of the user by capturing the brain impulses using an EMOTIV EPOC + 14 Channel electroencephalogram. This equipment has 128 Hz sampling frequency with 16-bit analog analog converter with 14 electrode channels: AF3, F7, F3, FC5, T7, P7, O1, O2, P8, T8, FC6, F4, F8 and AF4.

Electroencephalography (EEG) is an electrophysiological monitoring method to record electrical activity of the brain. It is typically noninvasive, with the electrodes placed along the scalp, although invasive electrodes are sometimes used, as in electrocorticography, sometimes called intracranial EEG. 
From EEG signals, several studies have presented the fact that EEG can be seperated in frequential bands each of them representing a specific behaviour:

* 𝛿 [ < 4 Hz] - deep sleep state
* 𝜃 [4 - 7 Hz] - task related to memory
* 𝛼 [8 - 15 Hz] - relaxation eye opened and closed
* 𝛽 [16 - 31 Hz] - physical activity, movment and excitation
* 𝛾 [ > 32 Hz] - nervous state, high activity and excitation

Then, if the signals energy is computed in each frequency bands. It is possible to represent an EEG into a vector of dimension = [𝑛𝑏𝑎𝑛𝑑𝑠×1] (here 𝑛𝑏𝑎𝑛𝑑𝑠=5). If we consider the total records with all the samples and channels, the feature vector has the following dimension [𝑛𝑡𝑟𝑖𝑎𝑙𝑠×𝑛𝑐ℎ𝑎𝑛𝑛𝑒𝑙𝑠×𝑛𝑏𝑎𝑛𝑑𝑠] with 𝑛𝑡𝑟𝑖𝑎𝑙𝑠𝑎𝑛𝑑𝑛𝑐ℎ𝑎𝑛𝑛𝑒𝑙𝑠 respectively representing the amount of trial and electrodes on the eeg cap.

The objective here is to recognize the brain activity which corresponds to one of the 4 activities that the participant is thinking about (muscle movements of the left   hands / muscle movements of the right hands / muscle movements of the left feet, and / right foot muscle movements).
