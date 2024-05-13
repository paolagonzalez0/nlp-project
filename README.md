# Predicting Movie Popularity and Revenue using BERT embeddings and Statistical Models

### Motivation
The global film and movie industry is a place where directors and producers can bring their ideas to life. However, in order to finance these movie ideas, they need investors who trust in the success of their movie. But what makes a movie successful? Does the description of a movie play an important role in its popularity or revenue? What about its genre? These scenarios and questions were just a few inspirations to create a model which predicts movie popularity and revenue based on many movie attributes including genre, movie description, release date, etc. This research provides a tool for directors and producers in the film industry not only to predict the popularity and revenue of a potential movie idea, but also provides a tool to convince investors to finance the movie idea. 

### Project Goals
In this project, I explore the creation of a statistical model to predict movie revenue and popularity based off of a movie’s characteristics. My main research questions were simple: Are we able to determine the revenue or popularity of a movie based on its description using statistical models? Does a movie’s plot and characteristics (genre, budget, language, etc.) determine its success in popularity or revenue? Can we gauge this success using statistical measures or is a more complex model needed to make a useful model? 

### Methodology
**Part 1: Exploratory Data Analysis**
- Clean and preprocess the data
- Explore the features
**Part 2: Machine Learning and Statistical Modeling**
- Create BERT embeddings for movie descriptions
- Prepare other features for statistical modeling
- Statistically model embeddings and features to predict a movie’s revenue and popularity
   - Calculate model performance
   - Visualize and compare model performance
   - Analysis and interpretation of model output
- Perform dimensionality reduction on the embeddings and features
- Statistically model PCA transformed embeddings and features
   - Calculate model performance
   - Visualize and compare model performance
   - Analysis and interpretation of model output
**Part 3: Future Exploration**
- Exploring the performance of more complex models 
   - BERTForSequenceClassification (with one class output)
- Explore other embedding implementations
   - Static Embeddings: Word2Vec, GloVe, etc.
   - Dynamic Embeddings: ELMo

### Results and Conclusion
In short, statistical modeling is not an effective way to predict movie revenue and popularity using movie characteristics. Although BERT embeddings are essential capture contextual information, they do not perform well under statistical modeling. This is most likely because of the high dimensionality of the embeddings. When used as features in regression models, these high-dimensional embeddings can increase the complexity of the model and the computational cost of training. Along with this, contextual word embeddings represent nuanced linguistic features and context-dependent meanings of words, making them less interpretable compared to more traditional word embeddings. In regression modeling, interpretability of features is often important for understanding the relationships between predictors and the target variable, especially when deciding which predictors should be kept in the model. Hence, a statistical model is not be the most effective type of model to predict movie revenue and popularity using movie description BERT embeddings.

