# Overview
This is for solving the classification of [Kaggle's Dogs vs. Cats](https://www.kaggle.com/c/dogs-vs-cats/data)

# Step to run on scrath with Google Colab
First modify the path to your google drive 
* *raw_train_dir* is the location of raw images for training
* *train_dir* is the location to store images which has been pre-processed and used to train the model
* *raw_test_dir* is the location of raw images for testing
* *test_dir* is the location to store images which has been pre-processed and used to test the model
* *train_data_file* is the location to store one big file has data of all the train images
* *train_label_file* is the location to store one big file has data of all train images' labels
* *test_data_file* is the location to store one big file has data of all test images
* *trained_model_dir* is the location to store the output trained models

After that run the **Prepare dependencies and global variables** block to load dependencies and prepare variables

Then uncommented code in **Transform to grey and store in trained set** and run it to pre-process both train and test images to *train_dir* and *test_dir*

Run **Dump data using pickle to avoid loading so many file for next run** to store data in one big binary file

Run **Prepare data to train** to prepare the data to train

The blocks **Train and save model with relu activation function**, **Train and save model with sigmoid activation function** and **Train and save model with softplus activation function** used to train the models with different activate functions and store the model in *trained_model_dir* at the end

Finally run **Get statistic of trained models** to get inside of the trained models statistic

# Step to run pre-trained models
Run the **Prepare dependencies and global variables** block to load dependencies and prepare variables

Run **Prepare data to train** to prepare the data

Run **Get statistic of trained models** to get inside of the trained models statistic

# Overview of used CNN models
Added later

# Processing flow diagram
Added later