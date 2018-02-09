#Overfitting:

	1. Early stop
	2. Data Augmentation
		- node, cropping, transformation of existing data
		- use Generative Model (VAW or GAN) on existing data, and sampling from the normal distribution

	3. REGULARIZATON:
		-  NOT TO HAVE A BETTER FIT
		- BUT TO COMBAT THE NOISE
		- WE KEEP THW W VALUES SMALLER
		- common : L2 regularization

	4. Dropout:
		- Ref: `Dropout: A simple way to prevent Neural Networks from Over fitting`
		- Combining smaller n/w together has better performance than one large network
    - `p for input data neuron must be close to 1 (0.8)`

  5. Batch Normalization:
		- Ref: `Batch Normalization: Accelerating Deep Neural Network Training by reducing internal covariate shift`
		- Normalization process is different during training and inference, need to specify in BN layer

   6. Pooling : Max pooling

## underfitting:
  - accuracy is declining in both training and testing phases
  - add more layers in the hidden layers
