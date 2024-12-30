# Trigger-Word-Detection

# Trigger Word Detection Project 🎤✨

## Overview
Trigger word detection is an exciting area of speech recognition technology that allows devices to respond to specific keywords, like "Hey Siri" or "Okay Google." This project has been an incredible journey, where we tackled various challenges and refined our model to improve accuracy. 🚀🔍 

## Model Architecture
By analyzing the **Conv1D** architecture and employing time-distributed layers, we effectively processed audio data to identify trigger words. 🎶💻 In our model, we start with a Conv1D layer that extracts features from the audio input. 🧠🔊 The **BatchNormalization** and **ReLU** activation functions help in stabilizing the learning process, while **Dropout** layers reduce overfitting. 🌈 

The first **GRU** layer captures sequential dependencies in the audio data, followed by another GRU layer for deeper learning. Each GRU layer incorporates Dropout and BatchNormalization to enhance performance. 📈💪 Finally, we use a **TimeDistributed** dense layer with a sigmoid activation function to make predictions for each time step in the sequence. 🕒🔮

## Audio Data Processing
To convert complex audio data into arrays for analysis, we utilize the **pydub** library, which simplifies audio manipulation. 🎧📊 By importing **AudioSegment**, we can easily load audio files and convert them
