# Recurrent Neural Network (RNN) 🧠



## ELI5 🧒
<details>
<summary>Click to expand</summary>

  
  
## What are RNNs? 🤔

Recurrent Neural Networks (RNNs) are a sophisticated class of artificial neural networks uniquely capable of processing sequences of data such as text, genomes, handwriting, or numerical time series from various sources. Unlike traditional neural networks, RNNs excel in applications where the sequence of data points is crucial, thanks to their ability to maintain a memory of previous inputs.

## Why RNNs? 🌟

In the digital age, data doesn't always come in independent packets. More often, it's a continuous stream of information where the sequence matters. Before RNNs, models struggled with sequential data, unable to leverage past information for future predictions. RNNs bridge this gap by incorporating a loop mechanism that allows them to retain a form of memory.

## How do RNNs Work? 🛠️

RNNs introduce a loop within themselves, processing data sequentially while retaining a memory (hidden state) of what has been computed thus far. This process allows RNNs to utilize previous computations (memory) in conjunction with the current input, a significant leap in handling sequential data.

1. **Loop Mechanism:** Combines current data input with the output from the previous step.
2. **Hidden State:** Acts as the RNN's memory, updated with each step, carrying information learned from prior inputs.
3. **Output Layer:** Depending on the task, outputs can be generated at each step or at the sequence's end.

## Challenges with RNNs 🚧

- **Vanishing Gradient Problem:** Training RNNs is notoriously challenging due to gradients diminishing as they are propagated back through time, complicating the learning of correlations in distant events.
- **Long Sequences:** The vanishing gradient issue makes it difficult for RNNs to process long sequences effectively, often losing context from earlier in the sequence.

## Applications of RNNs 📈

RNNs have proven effective across a variety of domains, including:
- Text generation
- Speech recognition
- Language translation
- Time-series forecasting

This introduction sets the stage for exploring more advanced models like LSTM and GRU networks, which build upon the foundational concepts of RNNs to address their limitations and enhance their capabilities. 🚀

</details>

# Predicting Median Daily Temperatures in Albury

## Overview🌦️ 

This project outlines the process of training a Recurrent Neural Network (RNN) using TensorFlow and Keras to predict median daily temperatures in Albury based on historical weather data. The project is structured in a sequential manner, covering data loading, preprocessing, modeling, training, prediction, and visualization of results.

## Project Structure 🛠️

1. **Initial Setup**: Import necessary libraries and set up the environment.
2. **Data Loading and Preprocessing**: Load the weather dataset, clean it (removing NaNs for MinTemp and MaxTemp), and create a new feature, MedTemp (median temperature). The dataset is filtered for Albury location.
3. **Data Visualization**: Plot daily median temperatures in Albury.
4. **Data Preparation for Modeling**: Scale the median temperature data using MinMaxScaler and split it into training and testing datasets. Define a helper function to reshape the data into a format suitable for RNN input.
5. **Model Building**: Define a Sequential model with a SimpleRNN layer and Dense layers.
6. **Model Training**: Compile and train the model on the training dataset.
7. **Prediction**: Use the trained model to make predictions on both training and testing datasets.
8. **Evaluation and Visualization**: Evaluate the model's performance using the Mean Squared Error metric and visualize predictions alongside actual data for both training and testing phases. Extend predictions to future dates.

## Data Description 🚀

- **File**: `weatherAUS.csv`
- **Columns**: 
  - Date
  - Location
  - MinTemp
  - MaxTemp
  - MedTemp (Derived)
  - Other weather parameters...

## Prerequisites ⬇
- Python 3.8+
- pip or conda
- TensorFlow 2.x
- Keras
- Pandas
- NumPy
- Scikit-learn
- Plotly

## Running the Code ⚙

To replicate this project:

1. Ensure you have Jupyter Notebook installed or use Google Colab for an easier start
2. Install necessary libraries: TensorFlow, Keras, pandas, numpy, scikit-learn, plotly.
3. Download the `weatherAUS.csv` dataset.
4. Run each cell sequentially to observe data preprocessing, model training, and evaluation steps.


## Results 📈

📊 The trained RNN model demonstrates promising results in predicting median daily temperatures in Albury. Evaluation metrics such as Mean Squared Error indicate the model's performance, and visualizations provide insights into the model's predictions compared to actual data.

## Contributing 🤝

Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are greatly appreciated.

- Fork the Project
- Create your Feature Branch 
- Commit your Changes 
- Push to the Branch 
- Open a Pull Request

## Acknowledgments 🌟

- TensorFlow and Keras Teams for providing the powerful libraries to build neural networks.
- The Australian Government Bureau of Meteorology for providing the weather dataset.
- All contributors who have helped in refining the project and extending its capabilities.

