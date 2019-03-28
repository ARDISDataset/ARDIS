#                                                 THE ARDIS DATASET of Handwritten Digits

#####                                                Huseyin Kusetogullari, Dept. of Computer Science, BTH
#####                                                    Abbas Cheddad, Dept. of Computer Science, BTH
#####                                                      Johan Hall, Arkiv Digital
#####                                                    Amir Yavariabdi, Dept. of Mechatronics, KTO Karatay
#####                                                     Håkan Grahn, Dept. of Computer Science, BTH


#### "ARDIS: A Swedish Historical Handwritten Digit Dataset", Neural Computing and Applications, Springer, 2019.

## I. Description of the Dat Sets

This is a new image-based handwritten historical digit dataset named ARDIS (Arkiv Digital Sweden). The images in ARDIS dataset are extracted from 15.000 Swedish church records which were written by different priests with various handwriting styles in the nineteenth and twentieth centuries. The constructed dataset consists of three single digit datasets and one digit strings dataset. The digit strings dataset includes 10.000 samples in Red-Green-Blue (RGB) color space, whereas, the other datasets contain 7.600 single digit images in different color spaces.

<img src="https://github.com/ARDISDataset/ARDIS/blob/master/ARDIS.png" width="500" height="400">

Further details of the ARDIS dataset can be obtained in our accepted paper:
#### Huseyin Kusetogullari, Amir Yavariabdi, Abbas Cheddad, Håkan Grahn and Johan Hall, 2019, "ARDIS: A Swedish Historical Handwritten Digit Dataset," Accepted for publication in Neural Computing and Applications, Springer.
#### DOI: 10.1007/s00521-019-04163-3

## II.  Acceptance of this Agreement

By downloading or otherwise accessing the Materials, Downloader represents his/her acceptance of the terms of this Agreement.


## III. References

If you use any of these data sets, please cite that as:

#### Huseyin Kusetogullari, Amir Yavariabdi, Abbas Cheddad, Håkan Grahn and Johan Hall, 2019, "ARDIS: A Swedish Historical Handwritten Digit Dataset," Accepted for publication in Neural Computing and Applications, Springer.
#### DOI: 10.1007/s00521-019-04163-3


## IV. ARDIS Dataset

#### ARDIS DATASET_IV: It contains 6600 training and 1000 testing images in .csv files. 

ARDIS_train_2828.csv
ARDIS_train_labels.csv
ARDIS_test_2828.csv
ARDIS_test_labels.csv

#### You can download DATASET_IV from the following link: https://github.com/ARDISDataset/ARDIS/blob/master/ARDIS_DATASET_IV.rar

We plan to upload the other data sets soon, stay tuned. 

## V. Implementation

#### DATASET_IV
#### In Python
x_train=np.loadtxt('.../ARDIS_train_2828.csv', dtype='float')

x_test=np.loadtxt('.../ARDIS_test_2828.csv', dtype='float')

y_train=np.loadtxt('.../ARDIS_train_labels.csv', dtype='float')

y_test=np.loadtxt('.../ARDIS_test_labels.csv', dtype='float')


#### reshape to be [samples][pixels][width][height]
x_train = x_train.reshape(x_train.shape[0], 1, 28, 28).astype('float32')

x_test = x_test.reshape(x_test.shape[0], 1, 28, 28).astype('float32')

## VI. Feedback or Comments

Please give us feedback/suggestions to improve the dataset.

Huseyin Kusetogullari: huseyinkusetogullari@gmail.com
Abbas Cheddad: abbas.cheddad@bth.se

Blekinge Institute of Technology
Karlskrona, Sweden on: 2019-03-28
