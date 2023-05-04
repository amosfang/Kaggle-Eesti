# Kaggle Eesti

## Object recognition for The Image Bank of Tartu

My work can be found on `tartu.ipynb`, using `ResNet34`.

### Build a model to improve the re-use and search of City of Tartu picture data.

Estonian government AI testbed competition invites everyone with expertise in data science and analysis to join an experimental testbed to find solutions to real-world problems using open data. We look forward to welcoming a range of specialists to come and work with us and become part of one of the most technologically advanced government projects in Europe contributing to the development of AI Gov stack that benefits the people across the globe. The AI testbed competition encompasses various works in the fields of data science, machine learning, and language technology, that open a way to contribute and become a part of developing the open-source AI Gov-stack.

Pick a competition you are interested in and help us to build the coolEST and brightEST digital state!

## Background
Tartu or as it is also known as “The City of great thoughts” is the second most populated city in Estonia. It is famous for its university, rich history and aspiration to innovate, and make citizens’ lives better.
Tartu has its own image bank, which contains 134 000 images divided into folders by the general topics. Unfortunately, images are not systematically labeled, which makes searching for the right picture complicated.

The accurate prediction model would help Tartu to make the public images searchable and reusable.

## Goal
The goal of this competition is to label the images from the image bank of the city of Tartu.

## Praise
* The best solutions will be publicly introduced to Estonian public sector.
* The best solutions become a part of Estonian e-government code repository.
* Social impact by creating a solution which would benefit a society as a whole.
* Chance to virtually meet top Estonian data scientists and build your network.

# Dataset Description
## Files
### `images.zip`
The compressed folder with all the images used in this challenge.

### `labels.csv`
This file represents the unique labels that you should try to link to images. (NB: you should only link images with the labels found in this file). The file has 2 columns:

* `label_id` - the unique identifier of the label (should be used in the list of labels that you provide as the result variable).
object - object that corresponds to this id (defined by human specialist).
train.csv
Training set that should be used to build your machine learning models. The training set includes both the image identificator and the ground truth about the labels of the image:

*  `image_id` – the id of the image (the image names match the ids),
labels – space separated list of label ids that correspond to this image.
test.csv
Test set should be used to see how well your model performs on unseen data. The test set includes the image_id but not the labels of the image. It is your job to predict the labels using the model you built on the training data!

### `sample_submission.csv`
An example of what the submission file should look like. For every row in the test data, submission files should contain two columns: image_id (representing the id of the image) and labels (a space separated list of the labels of the image). Example format:

`image_id`, `labels`

`img102`, **l0** **l1** **l41**I 

`img103`, **l44**

Etc.

In the example above, we say that image with id img102 includes labels **l0**, **l1** and **l41**. All unique labels are described in `labels.csv` (read more under data section).
