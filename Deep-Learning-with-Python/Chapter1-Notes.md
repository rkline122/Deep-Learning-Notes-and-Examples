# Notes on "Deep Learning with Python" by Francois Chollet

## Chapter 1 - What is deep learning?:
* AI is described as <i>the effort to automate intellectual tasks normally performed by humans</i>
* <b>Symbolic AI</b> is when programmers handcraft a large set of explicit rules for manipulating knowledge
* Machine learning discovers rules for executing a data processing task, given examples of expected output and requires 3 things:
  1. Input data points
  2. Examples of expected output
  3. A way to measure accuracy<br><br>

* The "deep" in deep learning stands for the idea of successive layers of representations. "depth" refers to the number of layers.
* Layered representations are learned via models called <b>neural networks</b> 
* Think of a deep network as a multistage information-distillation process, where information goes through successive filters and comes out increasingly purified
* The <b>loss function</b> takes predictions of the network and the true target and computes a distance score, capturing how well the network has done.
We use this score as a feedback signal to adjust the value of weights in a direction that will lower the loss score.
* Don't believe the short-term hype, but do believe in the long-term vision.

* Other classical machine learning approaches:
  1. Probabilistic modeling (Naive Bayes)
  2. Kernal methods (Support Vector Machine (SVMs))
  3. Decision Trees and Random Forests<br><br>

* Deep learning completely automates feature engineering.
* Deep learning allows a model to learn all layers of representation at the same time
* 2 essential characteristics of how deep learning learns from data:
  1. The incremental, layer-by-layer way in which increasingly complex representations are developed
  2. The fact that these intermediate incremental representations are learned jointly<br><br>

* The entire ML and DS industry has been dominated by deep learning (For perceptual problems)and gradient boosted trees (for shallow learing problems)
* The Python library, Keras, is the current go-to deep learning solution for a number of start-ups, grad students, and researchers.



