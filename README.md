<h1> Deliverable 1</h1>
<h4>1) Team </h4>
 	<h4>a)  Members</h4>
		<li>Veda Samhitha Dyawanapally</li>
        	<li>Meghana Chikyala</li>
   		<li>Poornima Pulakandam</li>
        	<li>Amarnath Reddy Chinthapalli</li>
		<li>Pavan Kalyan Reddy Madatala</li>
  	<h4>b)  Communication plan to include project artifact repository</h4>
A communication plan was created to outline how project artifacts were stored and shared among team members. In this case, We have used Google Spaces as the primary platform for discussions, while Google Meet was used for virtual meetings. Additionally, a Git repository will be utilized to share project files and other relevant information. The frequency of group meetings will be based on the project deliverables.

			
<h4>2)  Selection of data:</h4>
	We have chosen this dataset from Kaggle.
<h4>DataSet Link:</h4> 
<h4>Kickstarter Projects:</h4>
https://www.kaggle.com/datasets/ulrikthygepedersen/kickstarter-projects
<h4>DataSet Description:</h4> 
The data set contains details about Kickstarter projects and whether they were able to achieve their funding goals or not.
<h4>3) Business Problem or Opportunity</h4>
<h4>Kickstarter Projects:</h4>
The dataset we have chosen is from Kaggle which gives the data related to the Startup Project. We can use this data to derive some descriptive visualizations like how many projects were successful, which country has invested more in these projects, and whether the Number of Projects being successful is increasing year by year, etc.
Also, we use Machine Learning techniques and statistical analysis to give accuracy of the state of the project whether it is going to be successful or not, and for developing accurate predictive models.
<h4> Domain Knowledge</h4>
AWS S3, AWS Sage Maker for Analytics and ML Process.
AWS Quick Sight for Creation of Dashboard Visualizations.


<h4>4) Research Objectives and Question(s)</h4>
<h4>Kickstarter Projects:</h4>
<li>Which category of projects has the highest success rate?</li>
<li>What is the overall trend of crowdfunding projects over time, and how does this vary across different categories?</li>
<li>How many projects were successful and how many failed? What is the overall success rate of Kickstarter projects?</li>
<li>What is the Correlation between the Goal, Pledged, and Backers attributes?</li>
<li>Are there any outliers in the dataset, in terms of extremely high or low amounts pledged, number of backers, or project goals?</li>
<li>How many projects were launched for each category with respective year?</li>
<li>What is the average funding goal and pledged amount for different categories and subcategories on Kickstarter?</li>
<li>Can we predict the success rate of a project (i.e., the percentage of its funding goal that is met) based on its category, subcategory, country, launch date, and number of backers?</li>
<li>How important are Categories in predicting the success of Kickstarter Projects?</li>
<li>How important are Sub Categories in predicting the success of Kickstarter Projects?</li>

<h1> Deliverable 2</h1>
<h4> Data Understanding </h4>
<h4>a) Exploratory Data Analysis </h4>
Exploratory data analysis was performed using AWS SageMaker. EDA helps to uncover insights and patterns within the data, validate assumptions, and determine the best approach to analyze the data.

<h4> b) Dashboard </h4>
<p>Dashboard instances displaying visualizations like pie charts, bar charts, word clouds, line graphs, outliers, and correlation graphs were made using AWS QuickSight. Research objectives are evaluated using these visualizations. Additionally, other plots were also produced using an AWS Amazon SageMaker notebook.</p>


<h4> Data Preparation </h4>
<p>The dataset was checked for any missing values and those were removed to ensure accurate analysis. To enhance the analysis, a new attribute called 'Duration_in_days' was created using the 'Launched' and 'Deadline' attributes. Additionally, null values were checked and examined for each column, as they can hinder the machine learning algorithm's ability to learn. Afterwards, each column's data was observed thoroughly, and statistical measures such as standard deviation, mean, maximum, and other distributions were analyzed to determine the evenness of the data distribution.</p>
<h1> Deliverable 3</h1>
<h4>Analytics, Machine Learning:</h4>
We have used Amazon SageMaker, Athena, and Glue, which are great tools for recognizing and understanding the structure of the data. Athena allows us to query the data in S3 using SQL, while Glue automatically crawls and catalogs the data and generates ETL code to transform it into a format that is suitable for analysis. By using these tools, we have gathered a better understanding of our data and ensured that we are using the best ML tools for our specific dataset.

Additionally, Amazon machine-learning technologies like SageMaker, Athena, and Glue can help extract insights from the data and build accurate machine-learning models that can drive better business decisions.
![WhatsApp Image 2023-05-04 at 10 15 20 PM](https://user-images.githubusercontent.com/123277087/236364973-05fc7130-d9f8-46d3-b4c1-efd3cf5a9d87.jpeg)
![WhatsApp Image 2023-05-04 at 10 16 50 PM](https://user-images.githubusercontent.com/123277087/236365102-9753b698-605b-43c5-982a-b0be02a4dca4.jpeg)
![WhatsApp Image 2023-05-04 at 10 17 10 PM](https://user-images.githubusercontent.com/123277087/236365128-3dfa10a6-dd84-4c45-8da6-363f6a380965.jpeg)
<h4>Evaluation and Optimization:</h4>
AWS offers a variety of machine learning models and analytic tools, and we have used logistic regression and random forest models. 
The likelihood that a binary dependent variable that is binary will take a specific value is predicted by a logistic regression model of the relationship between a binary dependent parameter and any number of independent variables. 
Regression, as well as classification, are handled by an ensemble learning method known as random forest. It functions by building multiple decision trees on various subsets of the data that are randomly chosen, followed by combining the predictions from each tree to create a final prediction.
<h4>Results</h4>
The accuracy of a machine learning model on the dataset can be a useful metric for evaluating the performance of the model. For our Kickstarter dataset, accuracy can tell you how well the model can predict the outcome of a crowdfunding campaign (i.e., whether it will be "successful," "failed," "canceled," or "suspended") based on the input features.

<h5>1. How important are categories in predicting the success of Kickstarter campaigns?</h5>
Feature Importance:
<img width="509" alt="image" src="https://user-images.githubusercontent.com/123277087/236366016-39727d39-4f3d-42c8-be92-cb442e7154c9.png">
<h5>2. How important are subcategories in predicting the success of Kickstarter campaigns? </h5>
Feature Importance:
<img width="629" alt="image" src="https://user-images.githubusercontent.com/123277087/236366147-72695e14-197c-4637-b9ad-779a510b2917.png">
<b>Model Accuracy Scores:</b>
<img width="449" alt="image" src="https://user-images.githubusercontent.com/123277087/236366267-de6b5c36-6684-4a72-a683-adedba8fb600.png">
Based on the accuracy results, the Random Forest and Logistic regression models performed the best with an accuracy of 96% and 89%, respectively. SVM had an accuracy of 88%. 

Considering the accuracy and other metrics, it can be suggested that the Random Forest model is the best option for predicting project success based on the available features.

The feature importance analysis revealed that the "Category" and “Subcategory” features have the highest importance in predicting the success or failure of Kickstarter projects.

Analyzing feature importance for category and subcategory can provide valuable insights into the factors that influence the success or failure of crowdfunding campaigns and can help guide decision-making and improve predictions in the future.

Based on these results, it may be beneficial to invest in Kickstarter projects in certain categories that have a higher success rate.

<h4>Future Work, Comments:</h4>
<ol>
	<li><b>What was unique about the data?  Did you have to deal with imbalance? What data cleaning did you do? Outlier treatment?  Imputation?</b></li>
	The dataset is unique because it provides a large and diverse sample of Kickstarter campaigns across different categories, subcategories, and years. This makes it a valuable resource for studying the factors that contribute to the success or failure of crowdfunding campaigns. 
Dealing with imbalance is an important issue when analyzing Kickstarter project data, as there is a significant class imbalance between successful and failed projects.
Data cleaning for Kickstarter projects typically involves removing duplicates, dropping irrelevant columns, and dealing with missing values.
Outlier treatment was also necessary for certain variables, such as the funding goal or number of backers. 
Imputation was used to fill in missing values in certain cases, such as when some variables were missing for only a small proportion of the observations.
	<li><b>Did you create any new additional features / variables?</b></li>
	In the initial stage of the project, we utilized AWS Athena and AWS Glue to locate the data and created dashboards in AWS Quicksight. In the Analytics and Machine Learning modeling phase, we employed regression models, such as linear regression, to present the data results. AWS SageMaker was used to generate the outcomes. Adding new attributes such as year and duration range helped extract additional information from the data and improved the predictive power of the model.
	<li><b>What was the process you used for evaluation?  What was the best result?</b></li>
	The analysis of the Kickstarter project dataset involved the use of various AWS resources, such as AWS Glue, AWS Athena, and AWS Quicksight. These tools were utilized for data identification and a better understanding of the data after pre-processing. The processed data was then transferred to AWS SageMaker for the application of Machine learning models to obtain the final results.
	<li><b>What were the problems you faced? How did you solve them?</b></li>
	During the initial stages of the project's creation, a few challenges were faced while working with the Kickstarter dataset. The pre-processing involved data cleaning and feature engineering to enhance the predictive power of the model. The dataset was sourced from Kaggle, and it was challenging to set it up on the AWS platform due to compatibility issues, especially generating schema in Glue after running the crawler in Athena. In conclusion, while the project presented several challenges, we overcame them by working collaboratively and leveraging the available resources to deliver a high-quality analysis of the Kickstarter dataset.
	<li><b>What future work would you like to do? </b></li>
	For future work, there are several other features, like project description, creator's background, social trends, etc., that can be included to improve the model's accuracy. Analyzing the success rate of campaigns across different states or cities can provide useful insights for creators looking to launch campaigns in specific locations. Additionally, if the dataset is expanded to include other countries, regional analysis could be conducted.
	<li><b>Instructions for individuals that may want to use your work</b></li>
	If individuals want to use our work for the Kickstarter project dataset, which is available from Kaggle, they should set up an AWS account with appropriate credentials. The next step is to load the dataset into AWS and set up AWS Glue and AWS Athena to preprocess the data. Once the data is preprocessed, they can use AWS SageMaker to run the Jupyter Notebook consisting of the code. The code consists of data cleaning, feature engineering, and model building. They can modify the code according to their requirements and run the notebook to obtain the results. All the requirements for the procedure are mentioned in the Github repository, and individuals can refer to it for any further assistance.</ol>







	








