
#    “ Job-related Training Recommendation system”



- DEMO : [Job-related Training Recommendation system](https://trainjobapp.pythonanywhere.com/)
- Kaggle :[Published On Kaggle](https://www.kaggle.com/sarahalghamdy/job-related-training)

## problem statement
- Continuous training is crucial for creating and maintaining the right skill-profile for the employees. I aimed to formalize the problem of training recommendation to the employee,  taking into account the employee’s training and work history.


## Summry 

#### About The Idea 
- There is a tremendous variety in the available trainings within an organization: technical, project management, quality, leadership, domain-specific, soft-skills, etc. Hence it is important to assist the employee in choosing the best trainings, which perfectly suits his/her background, project needs and career goals. For this project, I focus on creatin a training recommendation in an industrial setting.

#### About The Data 
- contains the percent frequency data associated with Education, Training, Skills  and Experience Content Model elements. It is displayed in 15 tab delimited fields and identified using the column names provided above. Item rating level metadata is provided in columns named N, Standard Error, Lower CI Bound, Upper CI Bound, Recommend Suppress, Date, and Domain Source. The 15 fields are represented by one row. There are a total of 107,626  rows of data in this file.
- Important Featurs : 
   -  Categories associated with the Education, Training, and Experience content area. Categories for the following scales are included: Required Level of Education (RL), Related Work Experience (RW), On-Site or In-Plant Training (PT), and On-The-Job Training (OJ).
   -  The on-the-job training method takes place in a normal working situation, using the actual tools, equipment, documents or materials that trainees will use when fully trained.
   -  On-Site Or In-Plant Training  method also involves employee training at a site away from the actual work environment. It often utilizes lectures, seminars, case studies.
  
#### About The Model 
- Recommendation systems predict the future preferences of users based on their previous interactions with the items or it  Identifies a set of N items that will be of interest to a certain  user ( top-N recommendation problem).  I used the Word2Vec techniques implemented in the gensim. The model is trained using the input data and the dictionary. The output of the technique is continuous vector representation of words, which can be used as features by different applications. Word2vec (W2V) methods come from the Natural Language Processing (NLP) community. They were designed to produce low-dimensional distributional word representations. Theywere successfully applied to recommendation to generate user and product embeddings as they can scale to millions of items.


# Data 


| Column name          	| Dataset                     	| Description                                                                                                             	|
|----------------------	|-----------------------------	|-------------------------------------------------------------------------------------------------------------------------	|
| job_id               	| training_experience_dataset 	| O*NET-SOC Code                                                                                                          	|
| title                	| training_experience_dataset 	| displayed O*NET-SOC job titles                                                                                          	|
| element_id           	| training_experience_dataset 	| Content Model Outline Position                                                                                          	|
| element_name         	| training_experience_dataset 	| Content Model Element Name - Education, Work Experience, On-Site or In-Plant Training , On-The-Job Training, and skills 	|
| scale_id             	| training_experience_dataset 	| Scale ID                                                                                                                	|
| scale_name           	| training_experience_dataset 	| Scale Name , Content Categories along with scale name example : Required Level Of Education (Categories 1-12)           	|
| category             	| training_experience_dataset 	| Percent frequency category- Category value associated with element                                                      	|
| data_value           	| training_experience_dataset 	| Rating associated with the O*NET-SOC occupation                                                                         	|
| N                    	| training_experience_dataset 	| Sample size                                                                                                             	|
| date                 	| training_experience_dataset 	| Date when data was updated                                                                                              	|
| domain_source        	| training_experience_dataset 	| Source of the data                                                                                                      	|
| normalized           	| training_experience_dataset 	| data_value normalized                                                                                                   	|
| category_description 	| categories                  	| Detail description of category associated with element                                                                  	|

# Content :
- Collecting Data
- Data Cleaning 
- EDA 
- Model 
   - The implemented demo [Created Online Demo](https://trainjobapp.pythonanywhere.com/)
- Conclusion 
- Future Work 


