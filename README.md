# INN_IJOC

Code for the article <em>Multi-Objective Linear Ensembles for Robust and Sparse Training of Few-Bit Neural Networks</em>
by A. M. Bernardelli, S. Gualandi, H. C. Lau, S. Milanesi, N. Yorke-Smith

The repository contains one python file only, that can be used to reproduce the tests regardin the MNIST dataset.


The PARAMETERS can be modified accordingly to the experiments

For every value in the list "different_p", the file produces 3*n*m + 1 .csv files
where n is the number of instances, namely "instances", and m is the number of different numbers of
training images, namely the length of the list "training_images"
Fixed the training images i and the instance j, the file produces
- labels_i_j.csv
    for every image used in the tests, how many networks labelled a certain image with a certain label
- test_inn_i_j.csv
    for every network of the ensemble, some infos about gap, time, etc., are collected
- test_inn_i_j_weights.csv
    for every network of the ensemble, the weights distribution is collected
The last file, test_inn.csv, contains results on accuracy and label statuses
