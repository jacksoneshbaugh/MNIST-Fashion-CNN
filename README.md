# MNIST Fashion Dataset CNN with TensorFlow

Jackson Eshbaugh &bull; CS 424 &bull; Spring 2025

**Abstract**: This notebook trains and tunes a convolutional neural network on Fashion-MNIST using `KerasTuner` with TensorBoard logging, early stopping, and checkpoint saving.

## Running the Model

To simply run the model, select "Run Pretrained Model" in the dropdown. Then, the pre-tuned model will be run. If you'd like to run through the tuning process again, say so in the dropdown.

## Results

The best model achieved a test accuracy of $ 92.52\% $, and the validiation set plateaued at around $ 92.91\% $. Although it didn't reach the $ 98\% $ we were (informally) aiming for, this model demonstrates excellence in clasifying the MNIST Fashion dataset.

In a second iteration, I would consider:

- adding a third convolutional block,
- using batch normalization,
- increasing the number of epochs (maintaining early stopping), and
- expanding the search space
  - tune batch size, kernal size, or even run more trials

However, the current model generalizes quite well and meets the core objectives of the assignment: hyperparameter tuning, checkpointing, early stopping, and reproducible evaluation.
