# Overfitting

1. Early stop
2. Data Augmentation
  - node, cropping, transformation of existing data
	- use Generative Model (VAW or GAN) on existing data, and sampling from the normal distribution
3. REGULARIZATON
  - Not to have a better fit
  - But to combat the noise
  - We keep the _W_ values smaller
  - common : L2 regularization
  - http://www.deeplearningbook.org/contents/regularization.html

4. Dropout:
	- Ref: `Dropout: A simple way to prevent Neural Networks from Over fitting`
	- Combining smaller n/w together has better performance than one large network

  - `p for input data neuron must be close to 1 (0.8)`
  - https://www.cs.toronto.edu/~hinton/absps/JMLRdropout.pdf

5. Batch Normalization:
	- Ref: `Batch Normalization: Accelerating Deep Neural Network Training by reducing internal covariate shift`
	- Normalization process is different during training and inference, need to specify in BN layer

 - http://proceedings.mlr.press/v37/ioffe15.pdf

6. Pooling : Max pooling

## underfitting
  - Accuracy is declining in both training and testing phases
  - add more layers in the hidden layers

* [slides](fastAI_week4.pdf)

#### References:
* https://www.youtube.com/watch?v=LxfUGhug-iQ&index=7&list=PLkt2uSq6rBVctENoVBg1TpCC7OQi31AlC
* http://neuralnetworksanddeeplearning.com/chap3.html
* http://www.chioka.in/differences-between-l1-and-l2-as-loss-function-and-regularization/
* http://cs231n.stanford.edu/reports/2017/pdfs/300.pdf (Data Augmentation)
