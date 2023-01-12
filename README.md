# LearningRatevsBatchSize
Experiments based on https://arxiv.org/abs/1711.00489 to achieve similar accuracies after same number of epochs.

Code references: https://pyimagesearch.com/2019/07/29/cyclical-learning-rates-with-keras-and-deep-learning/


Issues: There's no real mechanism to determine the number of batches for each batch size, the numbers you see currently in "batches" are just trial and error. I need some logic to determine the numbers programatically. The only logic is, the dot product of batch size and batches should be some multiple of the size of the dataset. How big the multiple is depends on how quickly we want to cover all batch sizes, i.e how many epochs.

