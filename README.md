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





