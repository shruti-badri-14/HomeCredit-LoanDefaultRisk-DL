# Home Credit - Loan Default Risk Assessment Using Deep Learning

### Data - Obtained from Kaggle

### Introduction

Predicting loan defaults with high precision is essential for financial institutions to
effectively manage risks and sustain the health of the financial ecosystem. Deep learning
techniques have emerged as a powerful tool in this domain due to their ability to handle
complex, non-linear relationships within financial data. Research has shown that these
methods can significantly reduce loan default rates, highlighting their potential in
improving screening and credit management practices. By leveraging vast amounts of data,
deep learning models enhance the predictive accuracy of financial risk assessments,
making them invaluable for early detection of potential defaults and minimizing losses.
The importance of these models is further underscored by their ability to adapt to
changing economic conditions and borrower behaviors, ensuring stability and robustness
over time without requiring frequent recalibrations.

Advanced deep learning approaches, such as Bidirectional Long Short-Term Memory (Bi-LSTM)
and Deep Neural Networks (DNN) with residual blocks, offer deeper insights into borrower behaviors
and risk factors by capturing temporal dynamics and sequences in financial data. These models
integrate techniques like regularization and dropout to prevent overfitting and improve generalization,
ensuring consistent performance across diverse datasets. By incorporating these sophisticated models
into financial risk assessment, lenders can make more informed and timely decisions, enhancing their
ability to predict loan defaults accurately. This not only improves financial outcomes but also
promotes greater financial inclusion by enabling more accurate and fair assessments of borrower risk.

### Results

In our analysis, we evaluated various deep-learning models to predict loan default risks for
Home Credit, focusing on individuals with minimal or no credit history. The models
compared included a Baseline model, Deep Classification Network (DCN), DNN with
Residual Block, Bidirectional Long Short-Term Memory (BiLSTM), and Deep Neural
Network with VGGnet-inspired block. These were assessed based on training and
validation losses, AUROC scores, and stability metrics.

The Baseline model exhibited the highest overall stability scores (Train: 0.423, Validation:
0.411, Test: 0.398) and maintained consistent AUROC scores across all datasets,
demonstrating its robustness and reliability in performance without complex features. The
Deep Classification Network (DCN) showcased strong performance, particularly in
stability and AUROC scores, suggesting its effectiveness in capturing both explicit and
intricate interactions in the data. The DNN with Residual Block displayed decent
performance metrics but lagged slightly in stability, indicating potential issues with
capturing longer-term dependencies or overfitting to the training data.

The Bidirectional LSTM (BiLSTM), despite its higher training and validation losses, showed competitive
AUROC scores (Train: 0.718, Validation: 0.700, Test: 0.702) and capitalized on its ability
to process sequences with context from both past and future data points, offering a
significant advantage in understanding temporal dependencies crucial for accurate
predictions.

Lastly, Deep Neural Network with a VGGnet-inspired block was adapted for
sequence data, showing moderate success but highlighting the challenges of applying
convolutional network architectures directly to sequence prediction tasks.
Each model has its strengths- the Baseline for its simplicity and stability, DCN for handling feature
interactions, BiLSTM for enhanced temporal analysis, and Deep Neural Network with
VGGnet-inspired block for experimenting with convolutional approaches in sequential tasks.
