# Chapter 5 Notes:

* The purpose of a ML model is to <b>generalize</b> - to perfrom accurately on new data
* A deep neural network achieves generalization by learning a parametric model that can successfully interpolate between training samples
* The fundamental problem in ML is the tension between optimization and generalization
    * To attain generalization you must first get a good fit to the training data
    * However, improving the fit to the training data will inevitably start hurting generalization
* It's essential to be able to accurately evalutate the generalization power of your model while developing it.
    * Keep a completely seperate test set for the final model evaluation since information leaks might occur
* First goal on a new project is to create a model that can overfit. Best practices for achieving this are:
    * Fine tuning learning rate and batch size
    * Leverage better architectures
    * Increase model capacity
    * Train longer
* After model begins overfitting, you want to improve generalization through model regularization. This can be done by:
    * Adding dropout/weight regularization
    * Use early stopping
    * Use a larger data set
