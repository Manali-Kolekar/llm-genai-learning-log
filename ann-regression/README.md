ANN for Regression — Power Plant Energy Output Prediction

Built an Artificial Neural Network (ANN) in PyTorch to predict the net hourly electrical energy output of a combined cycle power plant using four environmental parameters: ambient temperature, ambient pressure, relative humidity, and exhaust vacuum.

Dataset: UCI Combined Cycle Power Plant Dataset

Key Learnings

- Understood the importance of feature scaling for neural networks. Since the input features are on different numerical scales, training on raw values causes gradients to become uneven, making optimisation slower and less stable. Standardising the input features allows gradient descent to converge faster and more consistently.
- Learned that the target variable (y) generally does not require scaling for regression problems because the output layer is linear (no activation function). However, scaling the target can still improve numerical stability and sometimes speed up convergence for larger output ranges.
- Gained practical experience with the complete PyTorch workflow: data preprocessing, defining an ANN using "nn.Sequential", selecting an appropriate loss function ("MSELoss"), training with the Adam optimiser, and evaluating regression performance.

Next Steps

- Experiment with deeper network architectures and different numbers of neurons to study their effect on model capacity and overfitting.
- Compare optimisers such as SGD, AdamW, and RMSprop to observe differences in convergence speed and final model performance.
- Explore techniques like learning-rate scheduling, dropout, and batch normalisation to improve training stability and generalisation.
