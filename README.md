# self_assessment_small_project
# Data-Driven Self-Assessment:
### Readiness for Artificial Intelligence & Data Science (ADS) Degree at Green University of Bangladesh



---


Author: Naeem Shovon Shuvro
Date: 23/10/2025


---


Problem/ Objective:
Evaluate Naeem Shovon Shuvro's current readiness for ADS degree and
identify areas for improvement




# Self-Assessment Mini Project
### "Is my current skills and knowledge good for getting into Artificial intelligence and data science program and how can this program help me?"

### Introduction
Dear Dr. Muhammad Abul Hasan,

I'm escited to share this short, data-driven self-assessment I built to explore "Why pursuing ADS program is the path for me". Instead of simply describing my strengths, I decided to appreach this reflection by analyzing my own profile using clustering, visualization and improvement analytics.


(N.B- The profiles in the dataset are made up reason being not having any real data regarding this topic but scores on my profile are my honest opinions. As it is on of my first few project there will be alot of mistakes and I tried to explain which topics I know but don't understand how it works under the hood)

The goal of this mini -project is to:
  1. Assess my skills arcross key areas
  2. Use unsupervised learning (KMeans clustering ) to see how my      profileis compared to an "Ideal Cadidate".
  3. Identify my strength and weaknesses.
  4. Demonstrate any anlytical thinking and motivate to grow through data.

By turning self-reflection into a simple machine learning problem, I wanted to show not just my enthusiasm for this field but also my mindset on analytical thinking and problem solving.

## Installation

Install python 3.13.7

```bash
  pip install python
```
###Required Packages

numpy
pandas
matplotlib
seaborn
scikit-learn
adjustText

### Importing Dataset
Importing the GUB_students_self_assessment_scores csv file with pandas and making a Pnadas DataFrame.Setting the profile column as index.

.<img width="1694" height="506" alt="Screenshot 2025-10-23 173151" src="https://github.com/user-attachments/assets/bb95c5f9-417f-47ab-ad8e-3c25be8e032d" />


<img width="1589" height="790" alt="op1" src="https://github.com/user-attachments/assets/176c7b23-b9ac-4401-a2c1-5eb9c565c80e" />

From this above clustered bar chart we can see:
1. Different profile score on different skills.
2. Ideal Candidate has higher scores in every skill than others
3. Need Support profile has the lowest scores on every skill.
4. Naeem Shovon Shuvro's scroes are in between Ideal Candidate and Need Support profile's score except for "Confidence"!.

EDA Conclusion:
1. The dataset has very small sample size.
2. The dataset is clean no duplicates, 5 rows and 11 columns
3. As Naeem Shovon Shuvro's assesment is in the dataset with assessment of "Ideal Candidate", "Strong Candidate", "Developing but Promising" and "Need Support" we can use a Clustering algorithm like KMeans to answer the problem statement.



### Standardization, Clustering and Visualizing the findings

First we standardized the features makes the mean 0 and std 1 for each feature to prevent KMeans bias towards any feature. StandardScaler = (feature value - mean value ) / standard deviation.

Then we used KMeans(TODO:tho I get how it works,need to understand more about how it works under the hood) an unsupervised learning algorithm for clustering similar type of profiles.Cluster 2 represents Ideal Candidates Cluster 1 represents Need Support profiles.

<img width="706" height="552" alt="op2" src="https://github.com/user-attachments/assets/9a48d7f6-95e4-4f22-bc95-556f7575384a" />

### Cluster Validation with inertia and silhouette

<img width="562" height="435" alt="op3" src="https://github.com/user-attachments/assets/36f15bf7-16da-4ea1-b1bc-5e8b4ca38e7d" />

### Cluster Validation
in KMeans unsupervised learning there is no label to predict we cant evaluate error matrics we can evaluate how well separated are the clusters and determine the optimal cluster number from getting the best validation score.

Inertia - Lower is better shows how tightly grouped the points are
Silhouette - -1 t +1 and closer to +1 is better. Distict clusters from each other

(N.B- I could't find a good validation score for this made up small dataset. Need to learn more about validation for unsupervised learning. I know know about Inertia and Silhouetter TODO: learn about more validation techniques)

<img width="977" height="707" alt="op4" src="https://github.com/user-attachments/assets/2353f6ed-fc7c-43ad-be87-d6c85f1f2d47" />


From this horizonatal bar chart we can see:
1. Basic ML Knowledge (5), Teamwork (5), Confidence (3) highlighted in orange are the skills I feel less strong (below 6).

2. Skills where I feel more confident (above or equal to 6), highlighted in blue:  Math Skills (7), Programming Basics (7), Python Skills (7), English Communication (8), Analytic Thinking (8), Financial Readiness (8), and Creativity (8).


<img width="928" height="679" alt="op6" src="https://github.com/user-attachments/assets/2182cdb2-4f06-4eb2-9151-ce918821851d" />


<img width="968" height="549" alt="op7" src="https://github.com/user-attachments/assets/0b32eec0-ace3-411d-9621-ef4f229cbec5" />

 the first heatmap helps understand the relationships between skills in general within this group of profiles, while the second heatmap provides a concise visual overview of Naeem Shovon Shuvro's personal skill profile.

 Color intensity represents scores for each skills. Darker the color higher the score and ligher the color lower the score.

 <img width="810" height="615" alt="op8" src="https://github.com/user-attachments/assets/e7c097e6-cda0-4aeb-8734-d8fe519928e0" />

 



From the radar chart above we can see:
1. **Shapes**: The green area is the shape of "Ideal Candidate" profile and is the benchmark for each skills. My profile's shape is the red area.

2. **Area of strength relative to benchmark:** English Communication, Financial Readiness, Anatylic Thinking, Creativity skills are close or match to Ideal Candidate.Math Skills, Programming Basics and Python skills are reasonably closer to the benchmark.

3. **Area of Improvement:** Basic ML knowledge, Confidence, Teamwork and Time Management shows a noticable gap between "Ideal Candidate"'s skills.

(N.B- My visualization skills is not great I got some help from google colab gemini.TODO: more practice with matplotlib, sns, plotly)

<img width="1734" height="446" alt="Screenshot 2025-10-23 173344" src="https://github.com/user-attachments/assets/ce629fc3-b99a-45bb-b640-c9ba4d40c8dc" />


<img width="771" height="253" alt="Screenshot 2025-10-23 173355" src="https://github.com/user-attachments/assets/7714d60e-e4f0-42f5-96fb-b799e47300d9" />

## Reflection

This small project is my honest and data-informed view of where I stand and how I can imporve in my Machine learning and Data science journey.Also shows how ready I am to get into BSc in ADS program which will provide me improvements and mentorship I badly need if I'm allowed to get addited.


### Key Insights
- The Areas I'm most confident about are **Analytical Thinking**, **English Communication**, **Financial readiness** and **Creativity**
-My Developing Areas which will help me during the course are **Math Skills**, **Programming Basics** and **Python Skills**
-The areas I need a lot of help and mentorship are **Basic ML knowledge**, Time management, Team work and mostly Confidence.

### Why this department is the right fit
Studying in the " Department of Artifical Intelligence and Data Science" will help me:
- Deepen my technical understanding of ML, AI and Data analytics
-Apply theory through real-world projects and research initiatives
- Build confidence with teamwork, mentorshhip, and presentation opertunity
-Develop the mindset to turn complex data into something meaningful - not for jsut grades but for reaseach and impact.

### My improvement plan
THe improvement table above outlies the areas I need to focus more tho there is alot to learn from each areas and more new ones.If I get the oppertunity to admit I will have 2 months to prepare during that time:
- Take some beginner ML lectures from the free online resources.
- Make some small python projects.
- Try to end the "Hands-on machine learning with scikit learn, keras and tensorflow" book by Aurelean Geron and start Statistics for machine learning with R
-Strengthen my data visualization skills
-Improve confidence by discussing with others about your projects

## Closing Thoughts
This reflection is a glimps of how serioursly I am taking this oppertunity if given and how I am approaching learning and self-growth.
I believe that joining this program will give me the structure, mentorship, and the challenge to transform these insights into action,
and to grow into a capable, creative data scientist and human being.


##############################################################################


## FAQ

## Questions I asked myself during this project and tried to answer them from my little understanding on some topics(There are some unanswered questions need to solve those later)

#### Question Could I use any other learning algorithms to solve this problem?


Answer => There is no labels to predict things so the data is a unsupervised data. The problem is a clustering problem like finding similar groups perticularly which group "Naeem Shovon Shuvro" profile belongs to so no supervised learning algorithm for this.

#### Question Why KMeans? Could I use any other unsupervised algorithms?

Answer => Could probably use Hierarchical Clustering it would've showed dendrogram of similar profile. also Gausssian Mixture Models(GMM) it adds probability and will show how much similar to each group my scores are. Could've used all 3 algorithms and take the result from the best algorithm(??).TODO: Need to learn more about these algorithms and validation for next project.


## Authors

- [@NSSMovin](https://github.com/NSMovin)
