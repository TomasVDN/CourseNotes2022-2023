# Beginselen van Machine Learning // Principles of Machine Learning

H. Blockeel, Kimmig, De Raedt, Davis

Study material: slides + recordings + reader

Written exam, closed book, with formula sheet

### What is Machine Learning (ML)

In what context?
  - DLSS
  - Recommendation systems (amazon, youtube,...)
  - Self driving cars
  - Language Learning
  - And much more

Definition:
>ML is the study of how to make programs improve their performance on certain tasks from (own) experiences

With performance = speed, accuracy,...
     experiences = earlier observations

Useful for anything that we don't know how to program (computer programs itself)
Link to AI => computer solves hard problems autonomously

In ML, the key is data
  - Examples of questions & their answer
  - Observations of earlier attempts to solve some problems

ML makes use of inductive inference: reasoning from specific to general

AI != ML != Deep Learning

![ML landscape](../Pictures/ML1.png)

ML in typical form:
  - Input = dataset
  - Output = some kind of model
Ml in general form:
  - Input = knowledge
  - Output = a more general form of knowledge

A generic approach is to find informative features (lightness, width, length,...) then find a line.curve/hyperplane... to determine result (/!\ Not perfect => underfitting and overfitting)

## Different properties
### Predictive vs Descriptive
Predictive : learn a model that can predict a particular property /attribute/variable from inputs

ex: face recognition, spam filtering,...

![Predictive](../Pictures/ML2.png)

Descriptive: given a data set, describe certain patterns in the dataset

ex: analysing large databases,

### Multiple learning models:
  - Distribution learning  (see slide 31)
  - Function learning (see slide 32)

### Parametric vs non-parametric
### Explainable AI
XAI (explainable AI) refers to the study of AI systems that can explain their decision/whose decisions we can understand. 2 levels:
  - We understand the learned model used of decision making
  - we understand the individual decision


## Responsible AI: Challenges
Privacy preserving data analysis
Learning *safe* models: models that will not violate certain constraints that are imposed (no bias,...)
