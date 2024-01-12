Go to "code" folder

In this repo the preprocessed data for 10,000 images along with its corresponding questions and answers exists. Therefore if on linux you can skip to step 6.a.

DONT RUN preprocessing without downloading the dataset correctly. Skip to 6a. if preprocessed data already exists. 

1. Download Dataset at https://visualqa.org/download.html
(There is example.txt files with the correct name in each folder, just delete the txt files and replace with the correct files from the dataset with the correct name)
2. Put annotations in dataset\ann\ --> into train and val annotations respective. Call the files "ann_'whicheverset'.json". (Whicheverset = 'train' or 'val').
3. Put questions in dataset\qst\ --> into test, train and val questions respective. Call the files "multi_qst_'whicheverset'.json" and "open_qst_'whicheverset'.json". (Whicheverset = 'test', 'train' or 'val').
4. Put images in dataset\ann\ --> into test, train and val images respective. (No need to change names.) 
5. Run "preprocessing.ipynb"

Otherwise if the preprocessed data already exists -->
6a. Run "training.py"

If that doesn't work due to the paths then run:
6b. Run "preprocessing.py" then --> 6a.

Saved results can be found in "late_fusion" --> 
Saved model: --> ckpt
Logged loss: --> log

Note: The jupyter files works good on windows, the ".py" files works on linux. 

(To preprocess and evaluate on windows the paths and preprocess paths might need a change from frontslash to backslash.) 