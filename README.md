Implementation Steps:- 

Part I: Basic Neural Network (NN)

Implemented a fully connected neural network to perform binary classification on a provided dataset.

  1. Data Analysis: Performed initial statistics and handled invalid character entries using unique() and replace() functions.
  2. Preprocessing: Scaled numerical features and converted categorical variables via One-Hot Encoding.
  3. Data Splitting: Divided data into Training, Validation, and Testing sets (70:15:15).
  4. Architecture: Defined a multi-layer perceptron using nn.Module with ReLU activations and a Sigmoid output layer.
  5. Training Loop: Implemented forward pass, Binary Cross Entropy loss calculation, backpropagation, and weight updates using SGD/Adam optimizers .

Part II: Hyperparameter Optimization

Enhanced the base model from Part I by systematically tuning hyperparameters to achieve >75% accuracy.
  Tuning: Experimented with Dropout rates, number of layers, batch sizes, and different activation functions.
  Performance Tools: Integrated advanced techniques including:
    Early Stopping
    Learning Rate Schedulers
    Batch Normalization
    K-Fold Cross-Validation.
    
Part III: Convolutional Neural Network (CNN)

Developed a CNN to classify 36 different categories of $28\times28$ images.

  1. Data Handling: Utilized torchvision.datasets.ImageFolder and DataLoader for efficient batch processing.
  2. Architecture: Built a custom CNN with up to 10 hidden layers, incorporating Max Pooling and Dropout.
  3. Goal: Achieved a target testing accuracy of >85%.
     
Part IV: VGG-13 Implementation

Implemented the VGG-13 (Version B) architecture, adapted for the specific dimensions of the assignment dataset.

  1. Architectural Adjustments: Modified the input layer to handle image sizes other than the standard 224x224.
  2. Adjusted the final fully connected layer to match the 36-class output requirement.
  3. Training: Applied Dropout and Learning Rate schedulers as proposed in the original VGG research paper.
