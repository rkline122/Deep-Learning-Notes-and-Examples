# Chapter 2 - Mathematical Building Blocks

* A <b>category</b> in a classification problem is called a <b>class</b>
* Data points are referred to as <b>samples</b>
* The class associated with a specific sample is called a <b>label</b>

* The core building block of neural networks is the <b>layer</b>. Think filter for data
* Layers extract representations out of data fed into them.
* "Dense layers" == fully connected

* The compilation of a neural network requires 3 things:
    1. An optimizer
    2. A loss function
    3. Metrics to monitor during training and testing

* <b>Overfitting</b> is when models perform worse on new data than on their training data
* <b>Tensors</b> are NumPy arrays
    1. Rank-0 tensors (aka scalars) contain only 1 number
    2. Rank-1 tensors (aka vectors) is a 1-D array
    3. Rank-2 tensors (aka matrix) is a 2-D array
    4. Rank-3+ tensors is an array of matricies

* Tensors are defined by 3 key attributes:
    1. Number of axes (Rank)
    2. Shape
    3. Data type

* Real-world examples of data tensors:
    * Vector data - Rank-2 tensors of shape (samples, features)
    * Timeseries data/sequential data - Rank 3 tensors of shape (samples, timesteps, features)
    * Images - Rank-4 tensors of shape (samples, height, width, channels)
    * Video - Rank-5 tensors of shape (samples, frames, height, width, channels)

* Tensor operations:
    * Element-wise operations (addition, relu)
    * Broadcasting (a way for a smaller tensor to match the shape of a larger tensor)
    * Tensor Product (dot product) - only vectors with the same number of elements are compatible
    * Tensor Reshaping - rearrange its rows and columns to match a target shape (matrix transposition)

* Gradient-based optimization
    * Gradient descent is the optimization technique that powers modern neural networks
    * The derivative of a tensor operation is called a gradient
    * The gradient of a tensor function represents the curvature of the multidimensional surface described by the function
    * Stochastic refers to the fact that each batch is chosen at random.
    * The training loop works as follows:
        1. Draw a batch of training samples and corresponding targets
        2. Run the model to obtain predictions (forward pass)
        3. Compute loss of the model on the batch
        4. Compute the gradient of the loss with regards to the model's parameters (backward pass)
        5. Move parameters in the opposite direction from the gradient, reducing the loss on the batch. The learning rate is a scalar factor that sets the "speed" of the gradient descent process. 
        6. Repeat until the loss seems sufficiently low
    * Most efficent to run with mini-batches of reasonable size 
    * Momentum addresses two issues with SGD- convergence speed and local minimum

* Backpropagation is a way to use derivatives of simple operations to compute the gradient of arbitrarily complex combinations of these operations.
* Computation graphs treat computation as data (helps us visualize Backpropagation)
* Automatic differentiation automates the retrieval of the gradients (All you need to worry about is the forward pass)
    * Use GradientTape to achieve this in TensorFlow



















