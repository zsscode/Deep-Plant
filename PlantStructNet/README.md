# The Plant-StructNet

IEEE Transactions on Image Processing (accepted)


## Description

This is the implementation of our T-IP work with titled -- Multi-Organ Plant Classification based on Convolutional and Recurrent Neural Networks.

The project is open source under BSD-3 license (see the ``` LICENSE ``` file). Codes can be used freely only for academic purpose.

![demo](ezgif.com-resize.gif)

## Citation 
If you find this code useful for your research, please cite:
```sh
@inproceedings{leeetip,
  title={Multi-Organ Plant Classification based on Convolutional and Recurrent Neural Networks},
  author={Lee, Sue Han and Chan, Chee Seng and Remagnino, Paolo},
  year={Accepted},
  organization={IEEE Transactions on Image Processing}
}
```

## Dependency

* The codes are based on [tensorflow](https://www.tensorflow.org/)

## Dataset
* The PlantClef2015 dataset used has 1000 plant species classes. Training and testing data comprises 91759 and 21446 images respectively.

* All the training and testing images are grouped into their respective observation ID (Tagged in PlantClef2015 dataset). Note that, plant images captured from a same plant are tagged with different mediaIDs but the same observation ID.

* Please download the:

	1. Precomputed fc7 features [here](http://web.fsktm.um.edu.my/~cschan/source/TIP2018Plant/fc7_feature.zip).

	2. Preorganised observationID files ``` obs_mediaID.7z ``` from the Dataset folder. It consists of .Mat files that named after plant ObservationIDs. Each Mat. file consists of B cell that stores the information of the respective mediaIDs.

	3. Lists of ObservationIDs and ground truth species classes from the Dataset folder:
	* test_obs_list.mat
	* test_obs_class.mat
	* train_obs_list.mat
	* train_obs_class.mat


## Installation and Running

1. Users are required to install [tensorflow](https://www.tensorflow.org/) Library.

2. Users are required to download the necessary files and data according to the aforementioned dataset section for a fair comparison to our proposed models.

3. Users can train the model from scratch by running the main.py which includes ``` temp_createStruct2_2.py ``` and ``` Var_seq2seq_classification_bidirectRNN.py ```.

4. Users can test the trained model prepared in the 'model' folder.


Note that users are expected to modify the corresponding files to correct path to work properly. Enjoy!


## Feedback
Suggestions and opinions of this work (both positive and negative) are greatly welcome. Please contact the authors by sending email to ``` adeline87lee@gmail ``` or ``` cs.chan@um.edu.my ```

## Lisense
BSD-3, see ``` LICENSE ``` file for details.