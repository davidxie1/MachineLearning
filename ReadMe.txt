ReadMe file:

codeAssessShape.py

I don't have enough time to do grid_search, model_selection, skewed data adjustment.
I didn't do version prediction, but it should be easy.

Running command:

python codeAssessShape.py --training path_of_training_data.txt --test path_of_test_data.txt --prediction-results path_of_output_data.txt


Algorithm:
convert the classes to digit, using two dictionary: string->int, and int->string

Create a key words list. Generate the matrix for uas strings. For each uas, search for the key words, if it has, then the cell value in matrix should be 1.

sklearn.linear_model.SGDClassifiter is used to train and predict.
