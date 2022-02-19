## What is Explainable AI?

Explainable Artificial Intelligence (XAI) methods allow data scientists and other stakeholders to interpret decisions of machine learning models. 
XAI provide us with two types of information, global interpretability or which features of machine learning model are most important for its predictions. And local interpretability or which feature values of a particular instance most influenced the outcome and in what way. 

## Why do we need Explainable Artificial Intelligence?
AI based decision making is being increasingly used in our everyday lives. When we go to an online store the products suggested to us are determined by an AI model - most probably a hybrid of content based and collaborative filtering method. 
The disease diagnosis is another area where AI is also being increasingly used. Another field is finance, where our credit risk is most likely calculated by a machine learning model. 

However, machine learning models are often a black box. To reconcile this with desire and demands of humans to have decisions explained to them a new field has developed within AI area - Explainable Artificial Intelligence or XAI. 

## Who is also driving demand for XAI?
Apart from customers, a key stakeholder that is demanding XAI are regulators. Some of the regulations that have put "Right to Explanation" at the center are: 
- [GDPR](https://eur-lex.europa.eu/eli/reg/2016/679/oj)
- [Fair Credit Reporting Act](https://www.ftc.gov/enforcement/rules/rulemaking-regulatory-reform-proceedings/fair-credit-reporting-act) 
- [Equal Credit Opportunity Act (ECOA) ](https://www.ftc.gov/enforcement/statutes/equal-credit-opportunity-act) 
The fields where the regulators will be especially keen to enforce greater transparency of Explainable AI are finance and health. Both sectors can have a significant impact on our lives and will be therefore more strictly regulated than others. 

## What are the main methods for XAI?

### SHAP
The most well founded method for XAI is [SHAP approach](https://github.com/slundberg/shap). It is based on Shapley values, which use coalitional game theory to distribute payouts from a game. 

In case of applying Shapley values to machine learning problem, the "game" is prediction of ML model, the "players" in the game are input variables values for given instance and the "payout" is equal to prediction with baseline score subtracted. 

SHAP method has several excellent properties, among other: 
- local accuracy
- consistency
- missingness

The SHAP library which implements the Shap approach comes with several very powerful functions: 
- shap.summary_plot is very useful for displaying the most important features of a machine learning model
- shap.dependence_plot is similar to partial dependence plot and allows you to explore how the feature influencers the outcome prediction
- shap.force_plot is key to gain local interpretability information, which feature values had highest impact on outcome probability and in which direction. 

### LIME
[Explainable AI Consulting](https://www.alpha-quantum.com/) companies often use another well known approach for local interpretability of AI models results - [LIME](https://github.com/marcotcr/lime).

In Lime approach, one fits a linear model on the local data set around the data instance. The coefficients of this linear model (which is highly interpretable) are then used for assessing importance of different features on the outcome for this instance. 

LIME method are less stable than SHAP approach when it comes to stability of results, defined as the changes in explanation on small changes of input variables. 

### ELI5 
ELI5 is another valuable library. It provides both global interpretation (one can use e.g. permutation feature importance method for that) as well as local interpretation. 

### Partial Dependence Plot (PDP)
The first step in XAI analysis is determining the most important features, which shows the most important features. In the next step, we want to then know not only which features are most important but how exactly are they impacting the probability of specific outcome. Does for example probability for class 1 rises or falls with increase in variable 1. 

To answer this question one can resort to PDP approach, which outputs a chart showing how the outcome probability changes with specific feature. PDP are usually generated for 1 or 2 features at a time. A useful python library for generating PDP is [PDPBOX](https://github.com/SauceCat/PDPbox). 

### Permutation feature importance
One of the earliest methods for determining importance of features was permutation feature importance. In this approach, one permutates values of a single feature and calculates change in error of the model. Features where such permutation increases the ML model error are deemed to be more important. 

One important disadvantage of permutation feature importance is that the results may be misleading if we are using features that have high correlation. 

### Data Visualizations

An important to provide stakeholders in companies with accurate information regarding AI explainability is to present the stories with data visualizations. 
[Data Visualizations Consulting](http://www.datavisualizations.org/) has in general become an important field, as more and more companies rely on the power of visuzalizations to present their work both internally as well as to outside audience. One of the applications for explainable AI is to help content marketers better understand what is the reason why they rank high or low on search engines for given keywords. [Tools for finding keywords](https://unicornseo.com/) are very important for all those that want to improve their search rankings. 

### Product categorization, product tagging and trending products

Product categorization belongs to the text classification class of problems, where the goal is to classify given text to a given pre-determined class. 
Example of text classification model is .e.g sentiment classification. 
[Product categorization for stores](https://www.productcategorization.com/) is an important discipline of machine learning models. 
With text classification, your text is categorized based on a set of pre-determined classes which you have provided us. Based on the given training data, we model a comprehensive predictive model that has the ability to predict the class of an unseen document, with a small rate of error. The accuracy of a machine learning based system depends on proper selection of features and the quality of the training data, apart from an intelligent design of the predictive model.

[Product tagging for stores](https://www.producttagging.io/) A.I. analysis engine digests all textual information in  content automatically and accurately to tag relevant categories, sub-categories, brands, designs, models, prices, reviews, technical specifications etc. With a few clicks, you can tag your products to enable search, recommend products that might be of interest, and create a seamless experience across all retail locations your customers may visit.

[Products in trends](https://www.trendingproducts.io/) tells you which products are trending. Profit Genie compares search engine popularity of top products sold by 1+ million of shops to deduce trending products. This is particularly helpful since not all trends are numerous enough to be noticed by human eye, but can still be an opportunity for business.
Simply enter your search query (e.g. 'coffee maker') and the monthly trend graph will automatically find products with the greatest surge in popularity over the last 12 months, along with chart showing search popularity over the last 1 year.

What is trending?  Trending products are those that have experienced a surge in popularity in a defined period of time, as derived from data from 1+ million ecommerce shops. In order to provide this service, we analyze the past 12 months of search query performance for products from 1+ million shops, and visualise the result of our analysis on a single page. You can easily identify item categories with the most trending products, view the most popular brands and get an insight into all items with a growing popularity.

### AI Lead Generation
[AI Lead Generation](https://aileadgeneration.ai/) offers AI lead generation capabilities to find your customers.
 Instantly find and communicate with new leads and potential customers within your niche. We know that generating potential buyers is tough, but we've created a lead generation tool that does it for you! Our software uses artificial intelligence to find your best customers, match them with your products and services, and send them to you. Huge quality leads produced quickly - all at no cost to you!
 
 ### Website Categorization API
 
 An important part in today's world is classifying websites. This can be used for brand safety, online filtering or for building own platforms. Website categorization usually involves classifying websites according to IAB standard. Note that there were several revisions of IAB classification taxonomy through the years and you need to pay attention to which one you need. There is [a free website categorization API tool available](https://www.websitecategorizationapi.com/) which you can use to categorize your websites. 
 It is using a machine learning model for automated classification and offers an API for easier use as well as introductory examples. 
 
  ### Top shopify stores in given country
 
Online stores is a very competitive business with billions of USD realized in many verticals. An important of operating an online stores is knowing who your competitors are. Many of online stores use [Shopify](https://www.shopify.com/)  as their underlying platform, which offers many features and is a leading provider of features for ecommerce. It has become such a success that its market capitalization on stock exchange surpassed 100 billion USD recently. 

But back to online stores owners. How do they get to know their top competitors? One approach is to [search for top shopify stores in given country](https://www.onlinestores.ai/) and then drill down even more by searching for top shopify stores in given country and given vertical (Tier 1, Tier 2 and Tier 3) according to Google product taxonomy.


## Useful resources: 

Most important libraries for Explainable AI: 

[SHAP](https://github.com/slundberg/shap)

[LIME](https://github.com/marcotcr/lime)

[ELI5](https://github.com/TeamHG-Memex/eli5)

[PDPBOX](https://github.com/SauceCat/PDPbox)

[PyCEbox](https://github.com/AustinRochford/PyCEbox)

[Skater](https://github.com/oracle/Skater)

[deeplift](https://github.com/kundajelab/deeplift)

[interpret](https://github.com/interpretml/interpret)





