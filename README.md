# Movie-Review-Sentiment-Analysis
Instructions

Usage:
	java <Positive_Train_Directory> <Negative_Train_Directory> <Positive_Test_Directory> <Negative_Test_Directory>

Put the desired test reviews into separate folders, one for the positive ones, another for the negative ones.
In order to use the training set I have provdied, use:

	java posTrain negTrain <Positive_Test_Directory> <Negative_Test_Directory>


Output:
The output will show the accuracy for each of the two polarities, as well as an overall average.


Note:
It is important to know that the ratio between the positive test reviews and negative test reviews matters significantly.
It is best to keep the number of pos and neg test reviews the same, so that the computed probability of either polartiy happening is 1/2 for Naiive Bayes computations.

If you only want to test a single review and determine whether the code guesses positive or negative:
	1. Put the review into the positive folder
	2. Create an empty text file in the negative folder
	3. Run the program as follows: "java posTrain negTrain <Positive_Test_Directory> <Negative_Test_Directory>"
	4. If the overall accuracy is 1.0, the code guessed positive. If the overall accuracy is 0.0, the code guessed negative.
