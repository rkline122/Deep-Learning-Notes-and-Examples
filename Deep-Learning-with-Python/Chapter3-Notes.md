
# Chapter 3 Notes- Introduction to Keras and TensorFlow:

* TensorFlow is an industry-strength numerical computing framework
    * Can run on CPUs, GPUs, or TPUs.
    * Can automatically compute the gradient of any differentiable expression
    * Can be distributed to many devices, and export programs to various external runtimes

* Keras is the standard API for doing deep learning with TensorFlow.
* Key TensorFlow objects include tensors, variables, tensor operations, and gradient tape
* The central class of Keras is the Layer. A layer encapsulates some weights and some computation. Layers are assembled into models
* Before training a model, you must pick (specified via model.compile()):
    * an optimizer
    * a loss
    * some metrics
* To train a model, use the fit() method
    * This runs mini-batch gradient descent for you
    * Use it to monitor loss and metrics on validation data (sets of inputs the model doesn't see during training)
* Once the model is trained, use model.predict() method to generate predictions on new inputs
