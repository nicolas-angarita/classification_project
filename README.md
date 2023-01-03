# To Churn or not to Churn ?

# Project Goals

My goal is to identify key drivers of churn. To see which customers are at risk of churning, and make recommendations for changes, so that we can reduce the monthly churn rate and at the same time increase customer retention.

# Project Description

Anytime a business is struggling, they have to revert to the basic questions of business and answer who is the customer and what makes them stay or leave. In this case why does it seem like so many customers are churning. What are key drivers that are turning our customers away? Could it be the services we are providing, our pricing policy, our target market (age of customer, gender, etc.), or other drivers. We will analyze some of the drivers just mentioned to see if we can come up with a model to see what is causing our customers to chun. Once we have ran our models we will make recommendations on how to better retain our customers from churning in the future. 

# Initial Questions

 1. Do customers with partners and dependents churn more than those with no dependents?
 2. Does the type of contract a customer have make it more likley to churn?
 3. Are customers with DSL more or less likely to churn?
 4. Are Senior Citizens more or less likely to churn than non Senior Citizen?

# The Plan

 - Create README with project goals, project description, initial hypotheses, planning of project, data dictionary, and come up with recommedations/takeaways

### Acquire Data
 - Acquire data from Sequel Ace and create a function to later import the data into a juptyer notebook. (acquire.py)

### Prepare Data
 - Clean and prepare the data creating a function that will give me data that is ready to be explored upon. Within this step we will also write a function to split our data into train, validate, and test. (prepare.py) 
 
### Explore Data
 - Create at least two hypotheses, set an alpha, run the statistical tests needed, reject or fail to reject the Null Hypothesis, document any findings and takeaways that are observed.
 
### Model Data 
 - Establish a baseline accuracy
 
 - Create and train three classification models.
 
 - Evaluate models on train and validate datasets.
 
 - Evaluate which model performs the best and on that model use the test data subset.
 
### Delivery  
 - Create CSV file with the customer_id, probability of churn, and prediction of churn for each observation in my test dataset.
 
 - Create a Final Report Notebook to document conclusions, takeaways, and next steps in recommadations for customers churning. Also, inlcude visualizations to help explain why the model that was selected is the best to better help the viewer understand. 


## Data Dictionary


| Target Variable |     Definition     |
| --------------- | ------------------ |
|      Churn      | 1 is customer left |

| Feature  | Definition | Encoded |
| ------------- | ------------- | ------------|
| customer_id  | Unique id for each customer  |
| payment_type |
| gender_encoded | 0 if the customer is male| 1 if the customer is female | 
	
 
',
 'internet_service_type_id',
 'contract_type_id',
 'customer_id',
 'gender',
 'senior_citizen',
 'partner',
 'dependents',
 'tenure',
 'phone_service',
 'multiple_lines',
 'online_security',
 'online_backup',
 'device_protection',
 'tech_support',
 'streaming_tv',
 'streaming_movies',
 'paperless_billing',
 'monthly_charges',
 'total_charges',
 'churn',
 'contract_type',
 'internet_service_type',
 'payment_type'] 
 
senior_citizen	1 if customer is a senior citizen	
tenure	Months of tenure as a customer	int
monthly_charges	The customer's monthly bill	float
total_charges	The customer's total bills since they have been a customer	float
is_male		int
partner	1 if the customer has a partner	int
dependents	1 if the customer has dependents	int
phone	1 if the customer has phone service	int
paperless_billing	1 if the customer has paperliess billing	int
multiple_lines_yes	1 if the customer has multiple phone lines	int
online_security_no	1 if the customer has internet but no online security	int
online_security_yes	1 if the customer has online security add-on	int
online_backup_no	1 if the customer has internet but no online backup	int
online_backup_yes	1 if the customer has online backup	int




## Steps to Reproduce

 - You will need an env.py file that contains the hostname, username and password of the mySQL database that contains the telco dataset. Store that env file locally in the repository.

- Clone my repo including the acquire.py and prepare.py (make sure to create a .gitignore to hide your env.py file since it will have your credentials)

- Put the data in the file containing the cloned repo.

- Run notebook.

## Takeaways and Conclusions

Upsets occur in 1/3 of games
In games where the lower rated player moves first there is a 4% greater chance of an upset
Games that are rated have a 3% higher chance of an upset
Games with a "quick" time control (30 min or less) have about a 1 in 3 chance of upset
Games with a "slow" time control (60 min or more) have about a 1 in 5 chance of upset
The mean rating of players in a game is not a driver of upsets
The difference in player rating is a driver of upsets
A player's choice of opening is a driver of upsets, however its influence is complicated and I would need more time to discover what role it plays


## Recommendations
To increase the skill intensity of a game add to the length of time players are able to consider their moves
Based on the data longer time controls make it less likely for a less skilled player to beat a more skilled player