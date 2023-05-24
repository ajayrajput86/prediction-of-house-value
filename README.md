prediction-of-house-value
Machine learning model to predict house price with Lasso and Ridge model 
https://github.com/ajayrajput86/prediction-of-house-value

1.  Importing all require lib
2. Working with outlier 
3. Visualizing data with chart 
4. finding high correlation feature with correlation
5. converting categorical data in to numeric with get dummy
6. Train Test split
7. Feature scaling with StandardScaler
8. Feature selection with RFE
	-Ve R2 score mean model performing worst than mean value
9. Applying Ridge Regression
	Find best param (alpha) with gridsearcCV
	Ploting (Alpha vs mean absolute error)
	Alpha is 50 
	find score = R2
		y_train  r2 0.7598186125692196
		y_test  r2 0.7631988815621915
		RMSE : 39041.327136640924
		Coefficent filteing 
	
	Test for double value of Alpha
	Removing top 5 feature and find new top features

10. Lasso reggression model creation
		# plotting mean test and train scoes with alpha 
		{'alpha': 1000}
		y_train  r2 0.7561042239674792
		y_test  r2 0.7577291015843524
		RMSE : 39489.65345273759
		
		
	Test with double Alpha = 2000
		y_train	0.7469571357195988
		y_test	0.7438393125313012
		RMSE : 40605.88101387955
		Coefficent filteing 
	
	Find top 5 feature after removing current top 5 feature
	
11. Summary

