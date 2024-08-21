# Home Credit - Loan Default Risk Assessment Using Deep Learning

### Data - Obtained from Kaggle

### Introduction

In the realm of consumer finance, predicting loan defaults with high precision is critical
for lenders to manage risks effectively. Financial institutions increasingly rely on deep learning
techniques due to their ability to handle complex, non-linear relationships inherent in financial
data. Research highlights the importance of these methods: for example, a study [1] found that
loan default rates can vary significantly, noting a reduction from 9.5% to 2% in certain regions
due to improved screening and credit management practices.
The early detection of potential defaults is vital not only for minimizing losses but also for
sustaining the health of the financial ecosystem. Surveys by financial regulators and academic
studies underscore the potential of advanced predictive analytics in preempting financial
delinquencies. Deep learning models leverage vast amounts of data and have been shown to
significantly enhance the predictive accuracy of financial risk assessments, evidenced by
performance improvements in practical applications [2].
Moreover, the financial landscape is continuously evolving with changes in economic
conditions and borrower behaviour. It is crucial for predictive models to not only be accurate but
also robust over time. Stability in these models ensures that they remain effective without requiring
frequent recalibrations, which can be resource-intensive. This balance between accuracy and
stability is key to the deployment of reliable financial risk assessments.
The application of neural networks in loan default prediction provides foundational insights
into borrower behaviours and risk factors. Techniques like regularization and dropout are
integrated into neural networks to prevent overfitting and enhance model generalization. These
adjustments are crucial for maintaining the model's performance across diverse datasets and over
time.
Furthermore, sophisticated deep learning approaches such as Bidirectional Long Short-
Term Memory (Bi-LSTM) and DNN with residual block are particularly effective in capturing
temporal dynamics and sequences in data, which are indicative of a borrower's financial behaviour.
These models offer deeper insights and higher predictive accuracy, thereby enabling lenders to
make more informed and timely decisions.
By integrating advanced deep learning techniques into financial risk assessment, lenders
and banks can enhance their ability to predict loan defaults. This not only improves financial
outcomes but also supports greater financial inclusion by enabling more accurate and fair
assessments of borrower risk.

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
capturing longer-term dependencies or overfitting to the training data. The Bidirectional
LSTM (BiLSTM), despite its higher training and validation losses, showed competitive
AUROC scores (Train: 0.718, Validation: 0.700, Test: 0.702) and capitalized on its ability
to process sequences with context from both past and future data points, offering a
significant advantage in understanding temporal dependencies crucial for accurate
predictions. Lastly, Deep Neural Network with a VGGnet-inspired block was adapted for
sequence data, showing moderate success but highlighting the challenges of applying
convolutional network architectures directly to sequence prediction tasks.
Each model has its strengths- the Baseline for its simplicity and stability, DCN for handling feature
interactions, BiLSTM for enhanced temporal analysis, and Deep Neural Network with
VGGnet-inspired block for experimenting with convolutional approaches in sequential tasks.
