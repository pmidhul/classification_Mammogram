The test data evaluation of the model yielded exceptional results, with a test accuracy of 87%. This outcome is particularly impressive considering the small size of the dataset and the fact that the image patches were only 50x50 pixels, and the model was trained from scratch.

Furthermore, we discovered several key insights during the analysis:

In traditional Convolutional Neural Network (CNN) architectures, the number of filters typically increases progressively, following a pattern like 64, 128, and 256.

However, when we followed this conventional approach with our 50x50 input images, the accuracy on the test data was only 81%, and the validation graph showed significant fluctuations. The reason being that we lost neary half of the information after the first layer of CNN. Because the image dimention was reduced to 23x23.

By adopting a different filter configuration, specifically using 256 filters in each layer, we not only achieved a 6% increase in accuracy but also observed more stable fluctuations in the validation graph. This indicates that the model consistently generated accurate predictions.
