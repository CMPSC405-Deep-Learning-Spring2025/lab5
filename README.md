# Lab 5: Implementing and Analyzing Deep and Bidirectional Recurrent Neural Networks (RNNs) in PyTorch

## Deadline: April 15th at 2:30pm

## Summary

In this lab, you will explore, implement, and analyze deep and bidirectional recurrent neural networks (RNNs) using PyTorch. You will build and train both a Gated Recurrent Unit (GRU) and a Long Short-Term Memory (LSTM) network with multiple layers and experiment with bidirectional architectures to process a sequential dataset. This lab also requires you to perform data preprocessing and evaluate how architectural choices affect performance. 

You will present a 3-5 minute summary of your findings during the lab session on **April 8th at 2:30pm**.

## Learning Outcomes

- Implement and train deep GRU and deep LSTM models in PyTorch.
- Implement and analyze bidirectional RNNs.
- Perform data preprocessing on a sequential dataset.
- Analyze and compare the performance and learning behavior of different deep and bidirectional RNN architectures.
- Visualize and interpret the outputs of sequential models.
- Experiment with model variations such as sequence length, hidden size, depth, bidirectionality, and dropout.

## Resources

- Refer to [D2L's Deep RNN Chapter](https://d2l.ai/chapter_recurrent-modern/deep-rnn.html) for theoretical insights.
- Explore [D2L's Bidirectional RNN Chapter](https://d2l.ai/chapter_recurrent-modern/bi-rnn.html) for bidirectional concepts.
- Use [D2L's RNN Basics Chapter](https://d2l.ai/chapter_recurrent-neural-networks/index.html) for foundational concepts.
- Explore [PyTorch RNN Documentation](https://pytorch.org/docs/stable/nn.html#recurrent-layers) for implementation details.

## Step-by-Step Tasks

### 1. Data Collection and Preprocessing

1. Choose a sequential dataset. Suggested datasets:
   - Text (e.g., Shakespeare for character-level language modeling)
   - Time Series Data (e.g., temperature or stock prices)
2. Perform preprocessing:
   - Clean and tokenize the data.
   - Create input-output sequences with a defined sequence length.
   - Split the dataset into training and testing sets.

### 2. Implement Deep and Bidirectional GRU and LSTM Models

1. Create **four models**: a deep GRU, a deep LSTM, a bidirectional GRU, and a bidirectional LSTM.
2. Define the model architecture with the following parameters:
   - Input size (from your dataset's features)
   - Hidden size (e.g., 128, but experiment with other sizes)
   - Number of layers (e.g., at least 3 for a deep RNN)
   - Dropout (e.g., 0.3 for regularization)
   - Bidirectionality (for the bidirectional models)

### 3. Train and Evaluate the Models

1. Define the loss function (e.g., `CrossEntropyLoss` for classification or `MSELoss` for regression).
2. Use an optimizer such as Adam or SGD.
3. Train all four models and log the training and validation losses.
4. Evaluate and compare the accuracy (or other metrics) of all models.

### 4. Visualize Model Outputs

1. Plot the training and validation loss curves for all four models.
2. For sequential outputs (e.g., text generation), generate and display sample outputs from each model.

### 5. Experimental Variations (Choose at Least Two)

Conduct at least **two** of the following experiments and report your findings:

- **Vary Hidden Size:** Compare performance with different `hidden_size` values (e.g., 64 vs. 256).
- **Increase Depth:** Train models with 1, 3, and 5 layers.
- **Bidirectional vs. Unidirectional:** Compare deep vs. bidirectional models for both GRU and LSTM.
- **Dropout Regularization:** Compare results with `dropout=0` vs. `dropout=0.5`.
- **Sequence Length:** Analyze how model performance changes with different input sequence lengths.

## Presentation (April 8th at 2:30pm)

Prepare a **3-5 minute presentation** including:

1. **Model Overview:** Describe the deep and bidirectional GRU and LSTM architectures.
2. **Data and Setup:** Explain the dataset, preprocessing steps, and hyperparameters.
3. **Results:** Present training/validation losses and model outputs.
4. **Discussion:** Compare model performance and discuss experimental findings.

## Deliverables

1. **Python Program (`main.py`)** implementing all four models (can have additional `.py` files but must run from `main.py`).
2. **Report (`report.md`)** documenting:
   - Data preprocessing steps.
   - Model architectures and parameters.
   - Experimental results and analysis (including required variations).
3. A GitHub repository with a clear commit history reflecting your work.

## Evaluation Criteria

This lab follows contract-based grading. To receive an `A`, you must:

- Implement deep and bidirectional GRU and deep and bidirectional LSTM in `main.py`.
- Perform data preprocessing and clearly document it.
- Complete and submit `report.md`, including visualizations (e.g., loss curves, sample outputs).
- Conduct at least two experimental variations and analyze their impact.
- Regularly commit progress to GitHub.



