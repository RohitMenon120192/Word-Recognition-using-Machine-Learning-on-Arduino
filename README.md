# Word-Recognition-using-Machine-Learning-on-Arduino

Hot Word recognition using machine learning on Arduino.

Problem Statement: The project is designed to address the challenge of monitoring individuals suffering from mental health issues by focusing on the detection of specific verbal cues. The initiative targets real-time monitoring of five predetermined keywords indicative of the individual’s mental state, specifically "all," "must," "never," "none," and "only."

Objective: The primary objective is to engineer an embedded device capable of recognizing the five selected "hot words" ("all," "must," "never," "none," "only") efficiently. This device must be both compact and effective, ensuring it can operate continuously without necessitating intrusive monitoring methods.

Implementation: The implementation phase involved collecting 50 audio samples for each of the keywords ("all," "must," "never," "none," "only") from multiple participants to compile a comprehensive dataset. This dataset was subjected to audio preprocessing to normalize each sample to a one-second duration, which then served as the input for training a neural network. ShuffleNet was selected as the model architecture for its efficiency and suitability for embedded applications. After the training phase, the model underwent quantization to minimize its size and complexity, making it compatible with the TensorFlow Micro project framework. This optimized model was subsequently deployed onto an Arduino Nano BLE device, chosen for its compactness and BLE capabilities, making it an ideal platform for this application.

Challenges Faced: Key challenges encountered included ensuring the effective capture and preprocessing of audio data to maintain uniformity across samples and optimizing the neural network to fit the limited computational resources available on the Arduino Nano BLE.

Solution: To overcome these challenges, a stringent data preprocessing protocol was established to ensure consistency in audio samples. The selection of ShuffleNet for the model architecture, coupled with model quantization, proved essential in balancing performance with the resource constraints of the embedded device. This strategy facilitated the deployment of a machine learning model capable of efficiently recognizing specified hot words on a low-power device.

Results: The solution, implemented on the Arduino Nano BLE, adeptly recognized the designated hot words ("all," "must," "never," "none," "only") from voice inputs, enabling it to execute predefined actions upon detection. This achievement underscores the viability of embedding compact and efficient machine learning models within embedded devices for real-time monitoring and response applications.

Conclusion: In conclusion, this project effectively combines machine learning with embedded systems to monitor mental health through verbal cue detection on the Arduino Nano BLE. It overcomes technical challenges to recognize specific "hot words" in real time, offering a non-invasive, practical solution for mental health care. This achievement highlights the potential for compact, efficient machine learning models in real-time monitoring applications, paving the way for future innovations in embedded AI for healthcare.
