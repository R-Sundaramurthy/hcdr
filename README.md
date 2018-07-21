# IMPORTANT

You need to add the data files locally in a folder called "input". The files are too big for the upload on GitHub. 
Also, we are not allowed to upload them (Kaggle regulation). You can download the files from the Kaggle competition https://www.kaggle.com/c/home-credit-default-risk/data

No worries, if you keep the .csv files in the input folder on your local machine, 
they should stay hidden from git (since .csv is added to the .gitignore file). Hence, they should not get pushed to GitHub if you push as usual.

## Next steps / problems to be solved

- Include non-numeric values in the prediction by adding a binary variable (of value 0 or 1) for every possible value of the non-numeriv value (currently just numeric, non-missing variables from application_train.csv are used)
- Deal with missing values (which method to chose? e.g. fill NA's with mean of the variable, using mean(na.rm = TRUE), or try using the mice package )
- Understand ROC (the key criterion for this competition), how to plot and how to compute it so that we can optimize our modesl based on this criterion
- Improve logistic regression (why is it doing so horribly right now?)
- Feature selection (make sure the previously added features don't harm the model and really add value)
- Try 5-fold or 10-fold cross validation (instead of splitting application_train.csv 2/3 for training and 1/3 for test)
- Apply other algorithms (LDA, QDA, KNN, SVM, tree algorithms) 
- Use bagging, boosting, random forrests (for model aggregation)
- Consider using the other prediction variables (from other data files next to application_train.csv)

