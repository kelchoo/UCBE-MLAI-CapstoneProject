# UCBE-Capstone-Module24

### Capstone 2

## Project Title: Building an Machine Learning solution on Shopify's App Store in the aim of maximizing revenue, lower cost and reduce customer churn (stimulate and accelerate the Shopify Business Model)

 <img width="672" alt="image" src="https://user-images.githubusercontent.com/115063137/218932224-d15802db-aae9-4dde-8448-6e6437e8e41c.png">


Overview: In this module, I will be showcasing the actual ‘number crunching’ for my capstone project. I spent the time in creating and training models, as well as creating visualizations to make sense of my findings.

- Program learning outcomes addressed this module:

- Apply real-world tools to model and analyze real-world data

- Communicate foundational concepts about AI/ML

- Draw useful conclusions from real-world data

- Identify the best ML model to solve a problem

- Implement the ML/Data Science Life Cycle

I will show how I explore my data sources, test a few of the techniques, and come up with a solution or answer to your research question.

**Author: Kelvin Choo**

## Executive summary

### The research question you intend to answer (one sentence, if possible):
#### • As a Shopify Marketing Corporate Executive: 

#### What are the strategies based on the top app and categories in my app store should I take to maximize revenue and lower cost?

#### To tackle this question, we need to use various visualizations, models and data preparation and exploration techniques to answer the detailed questions:

#### how do I get a recommendation of the top app which I should focus my marketing expenses when using the monthly reports provided (as shown in the data source as extracted from Shopify’s website in the link provided below) based on the various features and attributes of each app currently available on my store at the start of a given month (assuming the files have been provided in the point below from Shopify’s internal database to the marketing team) so I can maximize revenues for each month ? 
#### Based on the numerous apps in the app store, how does Shopify lower the costs due to risks posed by apps and bad reviews, to build long term relationships with app developers and users that will help identify areas of improvement and risks to its revenue model due to criminal activities and bad quality apps on its store.

#### Background of the company and its app store business:

#### What is Shopify app and how does it work?

#### Shopify is a commerce platform that allows anyone to set up an online store and sell their products. Merchants can also sell their products in person with Shopify POS. Shopify started over ten years ago when our founder Tobi wanted to sell snowboards with his company at that time called Snowdevil.
#### Evaluating Shopify Apps, their Reviews, and the Developer -  the keys for Shopify's merchants to succeed:

example of a popular app used by Shopify merchants
<img width="711" alt="image" src="https://user-images.githubusercontent.com/115063137/219320540-776b9a14-daba-4447-84c8-2570ffbf79e0.png">


The purchase of the app begins with clicking on the Get Started button, and the login page to Shopify begins your process to buy the app


<img width="508" alt="image" src="https://user-images.githubusercontent.com/115063137/219320901-386fc07e-2ed9-4312-b760-d9fb1e1ce3ff.png">

#### One of the secrets to creating a successful Shopify storefront is to utilize apps, add-on programs that provide additional functionality to Shopify sites. With the Shopify App Store, site owners can customize how an online store runs and how customers and users interact with it.

#### What Does Shopify Charge App Developers?
#### Last updated on October 1, 2022 @ 10:33 pm (source: https://www.websitebuilderinsider.com/what-does-shopify-charge-app-developers/ )

#### As the world’s leading ecommerce platform, Shopify offers a lot of opportunities for app developers.Shopify has an App Store with over 2,000 apps that can be used to power businesses of all sizes. While the platform is free to use, there are certain fees that app developers need to be aware of.
#### For example, if an app costs $10, Shopify would take $2. This is in line with other app stores, such as the Apple App Store and Google Play Store.

#### The most important fee for app developers is the Shopify commission. When an app is sold on the Shopify App Store, Shopify takes a 20% cut of the sale.

#### In addition to the commission, Shopify also charges a transaction fee on all apps. This fee is 2% of the total sale price and is used to cover the costs of processing payments. For example, if an app costs $10 and is sold through the Shopify App Store, the developer would owe Shopify $0.20 in transaction fees.

#### Finally, Shopify also charges a hosting fee for apps that use its hosting services. This fee is $0.50 per 1 MB of data per month and is used to cover the costs of hosting and maintaining apps on Shopify’s servers. For example, if an app uses 2 MB of data per month, the developer would owe Shopify $1 per month in hosting fees.



The below data sources contains the following key attributes about the apps currently offered on Shopify website for its merchants to download, purchase and use for various purposes that include increasing sales, simplify processes for completing the sales and invoicing processes or even promoting its website and measure revenue and forecasts inventory and sales growth.

Data includes:  App Counts, App Store review, pricing hints, descriptions, review counts, ratings, the various pricing plans offered for app developers

## Rationale
Why should anyone care about this question?
1. Its important to address the question of who and what app/product is my main revenue driver. For any business that intends to thrive in the era of competition, keep its current customers, in Shopify's case- keeping its app developers and merchants on its site is key to ensuring the sales revenue growth and sustainability.
2. Understanding the risk areas of the business is critical in helping the business of merchant and app hosting in Shopify's case in reducing churn to its competitors but also to eliminate risks from fraud and customer dissatisfaction as you will notice from feedback provided through the app business (especially in the reviews of the apps downloaded and the developer feedback).
3. Both of the above factors help ensure that the app store continue to provide the tools to help its merchants succeed and build a solid ecosystem for both sellers and buyers to thrive in and help Shopify succeed in online ecommerce. Note, that this business model is acutely similar to that of any app store worldwide that needs both great content and creators of content to co-exist and provide useful inputs for both demand and supply to continue to co-exist in any online marketplace.


## Research Question
how do I get a recommendation of the top apps which I should focus my marketing expenses when using the monthly reports provided (as shown in the data source as extracted from Shopify’s website in the link provided below) based on the various features and attributes of each app currently available on my store at the start of a given month (assuming the files have been provided in the point below from Shopify’s internal database to the marketing team) so I can maximize revenues for each month ? 
#### question 1: who is my top monthly app and developer in terms of reviews submitted and downloads (user counts) ?
#### question 1.1 : With the above information, how does Shopify or any online app store host build a strong relationshop and help promote the developer and apps to help it grow its revenue and market share?

## Data Sources
What data will you use to answer you question?
Expected data source(s) : https://www.kaggle.com/datasets/usernam3/shopify-app-store?select=reviews.csv

### apps.csv
### apps_categories.csv
### categories.csv
### key_benefits.csv
### pricing_plan_features.csv
### reviews.csv


## Methodology
What methods are you using to answer the question?
Applying the methods CRISP-DM
<img width="676" alt="image" src="https://user-images.githubusercontent.com/115063137/218926683-f2e4e4ad-c4a0-4a8b-ae88-b47d8a873e59.png">
####  Business understanding – What does the business need?
#### Data understanding – What data do we have / need? Is it clean?
#### Data preparation – How do we organize the data for modeling?
#### Modeling – What modeling techniques should we apply?
#### Evaluation – Which model best meets the business objectives?
#### Deployment – How do stakeholders access the results?


### Step 1: Understanding the Data (Business Understanding)

To gain a better understanding of the data:
· Libraries are imported and aliased correctly
· Appropriate plots for categorical and continuous variables are utilized
· Demonstrates competency with pandas
· Demonstrates competency with seaborn
· Variables are sensible
<img width="349" alt="image" src="https://user-images.githubusercontent.com/115063137/218887704-144c1a55-3abd-45d6-9470-d1eeffa1cfca.png">

### Step 2: Read in the Data

Use pandas to read in the datasets` and assign to a meaningful variable name.

<img width="2076" alt="image" src="https://user-images.githubusercontent.com/115063137/218887834-f538d032-48d0-4e50-9751-a602a8219bcb.png">
Creating joins and merge data to create meaningful linkage between apps, reviews and categories 
<img width="1349" alt="image" src="https://user-images.githubusercontent.com/115063137/218887882-3eca82e7-2aca-400a-9b05-9881c2788583.png">

### Step 2.1 creating joins with pricing and categories and factorize the data for easy identification and joining the data.
<img width="986" alt="image" src="https://user-images.githubusercontent.com/115063137/218888259-1b43ba2c-f247-4788-b1a0-f5931f8c313a.png">


### Step 2.2 Creating dataframes with joined data

<img width="1374" alt="image" src="https://user-images.githubusercontent.com/115063137/218888481-4220c4d1-d1a1-480f-9d87-e47167495c8e.png">

### Step 3 Data preparation by building Visuallizations to answer the following questions: 
- how do I identify as an executive managing an app store, what are my top performing categories of apps in terms of reviews (total), positive ratings, create a summary scoring system to identify my top category of apps.
- identify possible revenue potential from these top reviews/purchases 
- recognize and point out clear risks to revenue

<img width="2075" alt="image" src="https://user-images.githubusercontent.com/115063137/218888614-bac8886c-c038-40cd-8b2a-8729b54619a3.png">

<img width="2080" alt="image" src="https://user-images.githubusercontent.com/115063137/218889069-447156e7-7fec-411c-8d73-4350d99469a8.png">

<img width="2087" alt="image" src="https://user-images.githubusercontent.com/115063137/218889125-95924139-ea0e-4b89-aef6-117a06acd54e.png">
As observed that the top categories are Store Design, Conversion, Marketing for which reviews are driving the response on merchants using Shopify apps to generate sales to their websites and storefront.
Here the top app reviews give us a preview of the potential apps that we need to confirm that the reviews are key to ensuring their sustainability.

<img width="2037" alt="image" src="https://user-images.githubusercontent.com/115063137/218889795-6f2ca81e-cd40-4e94-b223-2823c4457a3c.png">
The top categories as shown here above confirm the pricing structure that works best for app.

### Step 4 Understanding the Features (data preparation  and understanding)

#### Using the chart below, Shopify should do the following to improve its sales and app store engagement with its developers and merchants:
#### 1. for the top rated apps, bring them to the main home page for the app store at Shopify's web site, this encourages them to develop more improvements on their apps and bring more returned customers to Shopify as merchants with these top toolsets using the apps to market, design their stores etc.
#### 2. for the low performing apps in the low 3s ratings, Shopify should bring them in house to collaborate on development and use case workshops to work with its merchants to improve their app experience and provide better customer support and insight to their app development process.
Over time, such behaviors of the developers, app users and Shopify teams help solidify the app store ecosystem much like Andriod and iOS app stores.

<img width="1584" alt="image" src="https://user-images.githubusercontent.com/115063137/218898115-b1592de7-cc51-44a8-9047-9569093c2372.png">

#### Note: From the chart above, majority of the apps have a rating of 4 and above. 
#### But how can Shopify help bring the rest of these ratings up from a 3 to a 4 ?

#### This chart uncovers the possibility of eliminating all the apps with rating of 0 and 1s to make sure quality apps dominate the landscaoe and therefore provide cost savings of not hosting apps that are not productive or contributing to the revenues at Shopify.
<img width="1559" alt="image" src="https://user-images.githubusercontent.com/115063137/218898183-0d4e5a8e-4cf4-49ea-a58f-f86625786c39.png">
<img width="1332" alt="image" src="https://user-images.githubusercontent.com/115063137/218898221-3d30817d-a7e6-4e68-9937-80577f050b1e.png">
<img width="1560" alt="image" src="https://user-images.githubusercontent.com/115063137/218898301-04d2c9b9-af8d-4415-83ad-b27989e175ec.png">

<img width="1351" alt="image" src="https://user-images.githubusercontent.com/115063137/218898396-d4a0c0f3-1f65-43a5-bea5-86f9ebd83675.png">

#### Correlation helps build the confidence and understanding that the user rating for using the app is a great feedback loop for the developer and for Shopify to feel the pulse of the merchants using its app and provides good understanding through the words used in the review which we will cover next in our models and clustering techniques used.

### Step 5: Understand the task and modeling (Modeling and Evaluation)
Business Objective of the task:

- find a model that can explain success of the product/app.

Such model can increase campaign efficiency by :

-- identifying the main characteristics that affect success,

-- helping in a better management of the available resources

-- and selection of a high quality

-- and affordable set of potential buying customers.

#### we use a combination of Chi2 to break down the reviews as features driving the ratings and reviews of the app developed for Shopify's merchants.
#### Chi2 is the most common feature selection method, and itis mostly used on text data.  In feature selection, we use it to check whether the occurrence of a speciﬁc termand the occurrence of a speciﬁc class are independent. Moreformally, forgiven a document D, we estimate the following quantity for each term and rank them by their score. Chi2 ﬁnds this score using equation Where•N is the observed frequency and E the expected fre-quency

#### This takes the value 1 if the document contains term t and 0 otherwise

#### It takes the value 1 if the document is in class c and 0 otherwise
#### For each feature (term), a corresponding high Chi2 scoreindicates that the null hypothesis H0 of independence (mean-ing the document class has no inﬂuence over the term’sfrequency) should be rejected, and the occurrence of the termand class are dependent. In this case, we should select thefeature for the text classiﬁcation

#### Continuing to clean the data and scrub for redundant columns after merging continues to be important as we drive towards the solution
<img width="1578" alt="image" src="https://user-images.githubusercontent.com/115063137/218898914-799e3c70-cdb0-4fa5-9281-f4d3154253fb.png">

#### Compute chi-squared stats between each non-negative feature and class.

#### This score can be used to select the n_features features with the highest values for the test chi-squared statistic from X, which must contain only non-negative features such as booleans or frequencies (e.g., term counts in document classification), relative to the classes.¶

#### chi-square test measures dependence between stochastic variables, so using this function “weeds out” the features that are the most likely to be independent of class and therefore irrelevant for classification.


#### Using NLP techniques, Shopify executives can really understand how the words used in reviews can be "nuggets" for building customer loyalty and branding knowledge for the apps that are popular and the ones that are not can really get the feedback needed to understand what is causing poor take rate and downloads by merchants:

<img width="1577" alt="image" src="https://user-images.githubusercontent.com/115063137/218899162-479f1a0b-7e14-44f4-a357-efc79fb27148.png">

#### Overall for from a modeling standpoint: 
#### Use of classification models for clustering words in reviews

#### (provide interpretation and classification of emotions based on app store reviews submitted coupled with scoring of words using weights help predict the top reasons for low reviews)

#### - SentimentIntensityAnalyzer  (VADER is an unsupervised learning algorithm widely used in Sentiment Analysis)

#### VADER’s SentimentIntensityAnalyzer() takes in a string and returns a dictionary of scores in each of four categories:

#### negative
#### neutral
#### positive
#### compound (computed by normalizing the scores above

#### Note: VADER ( Valence Aware Dictionary for Sentiment Reasoning) is a model used for text sentiment analysis that is sensitive to both polarity (positive/negative) and intensity (strength) of emotion.

#### VADER sentimental analysis relies on a dictionary that maps lexical features to emotion intensities known as sentiment scores. The sentiment score of a text can be obtained by summing up the intensity of each word in the text. 

#### Using python code library : analyser.polarity_scores(body)["neg"])
#### For example- Words like ‘bad’, ‘useless’, ‘poor’, ‘worst’ all convey a negative sentiment.”

#### Lastly:
#### In TfidfVectorizer we consider overall document weightage of a word. It helps us in dealing with most frequent words. Using it we can penalize them. 

#### TfidfVectorizer weights the word counts by a measure of how often they appear in the documents.


#### 6. Results (Deployment)

With Vectorization, chi square and SentimentAnalyzer text search tools we can truly magnify the category of apps and the respective grouping of words that point out the risks to growth of the app store.
<img width="1462" alt="image" src="https://user-images.githubusercontent.com/115063137/218899617-ed57d52e-1754-49b3-b8be-6507eb154d4b.png">

<img width="503" alt="image" src="https://user-images.githubusercontent.com/115063137/218899646-0a01900e-be7f-4f5e-b6dd-56f4189778da.png">


<img width="1788" alt="image" src="https://user-images.githubusercontent.com/115063137/218899684-e49aac76-0b47-46af-8721-73ca59ac5358.png">

<img width="1747" alt="image" src="https://user-images.githubusercontent.com/115063137/218899761-51f6954c-ec6b-4f5a-9b5a-8bc21c51281f.png">

## Conclusion

### Looking at the table above, with the top apps and developers identified to drive the potential revenues and stickiness of the ego systems of apps, the company can now repeat this process at the end of each month to do the following and set this process to run in automated fashion through automation of data synthesis from its enterprise database and running python scheduled jobs to produce the reports above to:

#### 1. Maximize the revenue of looking at promoting the app on the above list more during the month ahead starting with the top app performer in the most categories. 
<img width="1395" alt="image" src="https://user-images.githubusercontent.com/115063137/218927614-c695bdbb-5805-4d72-8aef-78e80775f8b4.png">
<img width="1397" alt="image" src="https://user-images.githubusercontent.com/115063137/218927676-cfb919c6-e031-4609-b734-bb76648c4797.png">
<img width="1383" alt="image" src="https://user-images.githubusercontent.com/115063137/218927722-d34818c9-170e-48ec-8a9e-ff6dcab6af33.png">

<img width="1115" alt="image" src="https://user-images.githubusercontent.com/115063137/224927823-bf1d3cac-a947-405b-ad73-8c021aaa83c3.png">
<img width="1073" alt="image" src="https://user-images.githubusercontent.com/115063137/224927877-85598674-8dec-4258-aaf7-ce0156780003.png">

#### If you notice the large number of apps written and posted on the app store by developer Elfsight, it seems they produce lots of add on apps like  Instagram and google reviews to help build seller visibility and connection to their buyers and also promote their branding.

<img width="961" alt="image" src="https://user-images.githubusercontent.com/115063137/224928353-fe183b23-fc31-468c-9d7a-989342fe94a9.png">

#### Notably, Privy as the top developer of apps that cater to 3 significant categories of merchant engagement on Shopify definitely deserves a seat at the table with Shopify, its host, and with greater partnership and revenue sharing to develop more apps for its merchants, Shopify can entice its merchants to spend more money on apps which it stands to collect a great deal of revenue both from returned merchants as well as making use of site features to host their merchandise.

#### The Privy app and its Shopify app store download page which include reviews and pricing info, from the above analysis demonstrates and confirms that our analysis is accurate in terms of how this app and developer has made significant contributions based on its popularity to Shopify's revenues on a monthly basis and its relationship has lasted more than 7 years which is worth noting that we can use this app as an example of how we can improve the other apps and developers' approach to app development and customer relationship building.
https://apps.shopify.com/privy?search_id=ae99b6ac-3774-4887-958d-d7c5f05548d1&surface_detail=Privy&surface_inter_position=1&surface_intra_position=1&surface_type=search

<img width="1167" alt="image" src="https://user-images.githubusercontent.com/115063137/219322130-13a0db70-e8bb-43ca-8095-83127fb96b89.png">

<img width="1153" alt="image" src="https://user-images.githubusercontent.com/115063137/219322467-b3dca213-cd28-47cd-a209-40608e398d45.png">

#### 2. focus more on the risk area in terms of investing on reducing fraud
#### - looking at the reviews, Shopify should acknowledge it needs to work closely with its developers on the apps side to close the potential of scammers coming through and destroying ths trust and safety elements that keep its profitablility and market share growing. As such, by deploying the above mentioned process of generating prescriptive and discreptive analytics of its app reviews by category and identifying the app developers that need to be removed from its site or encouraged to improve it practices and app security and integration, Shopify can reduce customer churn and reduce cost to fraudulent activities.

<img width="581" alt="image" src="https://user-images.githubusercontent.com/115063137/224933833-63ac9666-f213-4dd3-95c4-2adcdec8edea.png">

#### - This would in turn reduce merchant complaints, refunds and revenue loss to criminals and customer churn.
<img width="889" alt="image" src="https://user-images.githubusercontent.com/115063137/224943389-1c7d1230-e95c-4df6-9729-e4b8cda0ed36.png">
#### -  In addition, its important to note that out of the lowest rated app developers, the majority have international origins based on their foreign language names and non LLC, and U.S. relateed incorporation as shown above,
Therefore, this finding shows Shopigy needs to implement some additional security measures and questionaires for foreign apps to evaluate the credibility of their sign up and country origin to prevent future fraud and scamming sellers and buyers account from happeninig.

####  3. improving Shopify's own apps based on the ratings and feedback provided through the repeated process above.
Shopify being one of the lowest top developers should focus on improving its technology and investing in partnering and learning from its developer base to grow its own apps capabilities to help its partners and merchants deliver and market merchandise more effectively to help grow its revenue.


#### 4. With NLP, the deployment model should be at the end of each month, the executive team needs to review the report provided on the review text search and report as shown in section 5 and 6 above to better understand if the the following has improved:
 #### a. fraud and scam rates from reviews reported
 #### b. customer satisfaction has improved
 #### c. numbers of ratings with 4 has increased through marketing efforts and collaboration between the Shopify team and among developers.
 

#### Outline of project
Link to Notebook: 

https://github.com/kelchoo/UCBE-MLAI-CapstoneProject/blob/main/Capstone24-1.ipynb



##### Contact and Further Information
#### Thank you to Matilde and Isaac for their invaluable support and feedback in multiple sessions to make this module a success and a very well rounded experience for me in the ML area when completing this Capstone project. Your patience and insights have been great in keeping me at the fore front of understanding the key elements of ML and the ability to apply them in the app store business cases. Stay tuned for more Capstone improvements coming your way on this page in Module 24 !
#### you can reach me for any further questions via your inputs on this site.
