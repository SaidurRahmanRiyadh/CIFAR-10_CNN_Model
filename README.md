# CIFAR-10_CNN_Model

The model is a convolutional neural network (CNN) designed for image classification, particularly on small images of size 32x32 with three color channels (RGB). It consists of three convolutional layers with ReLU activation, where the first layer has 32 filters and the next two have 64 filters, all using 3x3 kernels. Each convolutional layer is followed by a max-pooling layer with a 2x2 window to reduce spatial dimensions and improve computational efficiency. After feature extraction, the model flattens the output and passes it through a dense layer with 64 neurons and ReLU activation. Finally, the last dense layer contains 10 neurons, corresponding to the number of output classes, and does not use activation since it is paired with `SparseCategoricalCrossentropy(from_logits=True)`. The model is compiled with the Adam optimizer and tracks accuracy as a performance metric. This architecture is commonly used for image classification tasks like CIFAR-10, balancing depth and computational efficiency.
