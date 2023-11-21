# credit-risk-classification
this Supervised Learning exercise will train and evaluate a loan risk model.  Goal is to identify creditworthiness of borrowers.
overview of the analysis 
	purpose: the purpose of the credit risk is to minimize the lending services giving loans to borrowers who are of high risk to default on the loan. it will also improve on missing giving loan to borrowers are not high risk.
	this analysis takes the data and trains it to find high and low risk borrowers.
	
Results:
	accuracy score: The accuracy (0.9520479254722232) is pretty good.  
	precision score: the precision score it needs to be low as possible.   
	recall score: The logistic regression model prediction for the healthy loans shows as 99% will be correct. This means that for the healthy loans the model will predict 99% correctly and then the loan will be given. This is shown by the recall score of .99 The recall score for the high risk loans is point .91 means that out of 100 high risk loans the logistic regression model prediction will give a loan to 9 borrowers who may default on a loan. Another way to say this, is 9 loans per 100 high risk loans may get defaulted. The lender should review these loan assignments more.

Summarized results 
	justification of recommending the model
	When checking the value counts for the balance of the target values; this step points out the that 0 (healthy loan) and 1 (high-risk loan) are UNbalanced by 72536. it would be hard to recommend this model since it is unbalance but i could recommend if the lender service understands its limitations. 
	
		
Credit Risk Analysis Report
overview of purpose of analysis
	the logistic and resampled training improves the model but appending more data from existing data to the unbalanced data.  this is done by using the RandomverSampler and now both training set are even at 56271 records.

Results:
	accuracy score: the accuracy is improved from 95 to 99!
	precision score: the precision score went down to .84. the precision score it needs to be low as possible.
	recall score: recall improved both for positive and false positives both Recall are at 99%. the RECALL for the 0 (healthy loan)is at 99% but more importantly the RECALL for the 1 (high-risk loan) went from incorrectly giving 9 out 100 to risky borrowers to now only giving 1 out 100 risky loans.
	
Summarized results 
	this model will accurately predict  the 0 (healthy loan)is at 99% and 1 (high-risk loan) at 99% correctly. i can now recommend this model.

Below article used for understand on confusion martix, precsion and  recall.
https://towardsdatascience.com/performance-metrics-confusion-matrix-precision-recall-and-f1-score-a8fe076a2262
Tutoring assisted with understanding of randomoverSampler and machine learning concepts also
