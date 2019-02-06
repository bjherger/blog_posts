# Rocking Data Science Interviews

Interviews suck. Interviews are an inefficient and biased way to determine evaluate an person's skills and qualities, 
and data science interviews in particular tend test for wrote memorization. Fortunately, this test covers a relatively 
small and standardized set of concepts, which makes it easy to brush up, and bring your A-game to an interview.

Below is an (inexhaustible) list of the concepts I've used to design my own interviews, heard from colleagues, or have 
seen in the wild. I won't promise that this will land you your next job, but it should be a good place to start your 
review.    

## Machine Learning

Modeling and machine learning is a large domain, with many overlapping and / or esoteric sub-domains. I'd recommend 
firming up the standard areas, as well as a few specialized areas

 - Class imbalance: How to deal with classification projects where one or more response classes is rare
 - Classification metrics: How to evaluate classification models when data has class imbalance
 - Anomaly detection: Determining if observations or 'irregular'
 - Time series: Modeling on data sets involving timestamps or snapshots of the same 'item' at different times 
   - Dummy out: Converting timestamps to dummy variables (e.g. day of week, month of year, AM / PM)
   - ARIMA: Models ocusing on predicting future values from lagged (previous) values of the same variable. 
   Auto-regressive (previous values) integrated (delta between previous time 
   steps) moving average (previous errors)
   - Proportional hazard (AKA time to live models): Determining how long until an event occurs (e.g. how long until a 
   patient dies or a region experiences a flood) 
 - Variable importance: Why do I care about this variable? Should I include it?
 - Model deployment: Great, you built a thing. Now how do we ship it?

### Linear regression

 - BLUE: If the gauss-markov conditions are met, OLS is the best linear unbiased estimator
 - L1 (Lasso), L2 (Ridge) normalization: Suggesting the the OLS model reduce coefficients towards zero, by adding 
 coefficients into the cost function. L1 adds the absolute coefficients, L2 adds the coefficients squared 
 - Elasticnet normalization: A combination of the L1 and L2 loss terms, using a linear interpolation
 - Model interpretation: What's the model trying to say? 
 - Variable importance: What are the betas trying to say?
 - p-values: Probability that coefficient is zero. If p-value is below alpha (usually alpha=.05), then we reject the 
 null hypothesis that beta = 0.  
 - R^2: How much of the variance in the data is explained by the regressors?
 - Adjusted R^2: How good is the model? How much of the variance in the data is explained by the regressors, while 
 penalizing for throwing in as many variables as possible?
 - Common issues
   - Endogeneity: Errors correlated with a regressor
   - Heteroskedasticity: Variance of errors is correlated with a regressor
   - Multicollinearity: Regressors are linear combinations of other regressors
   
### Model selection

 - Train / test / validation split
 - Grid search
 - Cross validation
   - Leave one out cross validation
 - Stratified sampling: Maintaining the proportion of response variable classes in different data samples
 
### Classical NLP

 - Tokenization: Breaking your string into distinct 'words' (tokens)
 - Ngrams: Capturing adjacent tokens, to capture adjacency and minimize the effects of breaking things into a bag of 
 words 
 - Bag of words: Breaking up your string into word (token) counts
 - TF-IDF: Assigning a weight to each word based on how 'canonical' it is to the document at hand, or all of the documents 
 - Cosine similarity: A measurement for how 'similar' two words are, usually based on TF-IDF vectors. Each document 
 will have a TF-IDF score for each word in the vocabulary 
 
 
### Deep learning NLP

 - Embedding: A mapping from characters or tokens to a vector
 - Recurrent neural networks: A specialized layer that can handle time series data, such as consecutive words in a text
 
### Deep learning

 - Neuron: The atomic unit for most neural networks. In it's simplest form, a Linear combination of the features in 
 the previous layer
 - Activation functions: An activation applied to the output of the neuron, to allow for non-linear relationships. 
 (e.g. linear, ReLU, softmax, sigmoid)
 - Layers: An abstraction that combines many similar neurons or functions (e.g. dense, dropout, convolutional, recurrent)

## Software engineering

The term 'Data Scientist' has many uses in the wild, ranging from purely research positions to software engineering 
positions with a dash of data. Regardless of how you define Data Scientist, I'd recommend beefing up your software 
skills, which can net another $10k-30k in salary.  

### Software engineering

 - Unit testing: Tests to confirm that atomic units of code act as expected
 - Integration testing: Tests to confirm that modules of code work together as expected
 - Continuous integration: Running tests and other quality metrics on code regularly, as it is developed and merged 
 into the code base
 - Continuous delivery: Developing code in short cycles
 - Continuous deployment: Frequent, automated code deployment
 - Service level agreement: The minimum (technical)specifications for a project, usually describing reliability, 
 responsiveness and features
 - Functional programming: A paradigm emphasizing programming functions as mathematical functions, and avoiding side 
 effects
 - Object oriented programming: A paradigm emphasizing organizing code around objects, and in particular attributes and 
 functions associated with those objects
 - Microservices: A paradigm emphasizing breaking down computations to small, atomic units. Each unit is treated as an 
 independent service
 - APIs: Application programming interface, a paradigm emphasizing the interface between programs or services
 - Lazy evaluation: Taking all of the instructions from the user, and ignoring the ones that they never check up on
 - Code versioning
 - Code commenting

### Databases

 - CRUD: The basic operations for a SQL database (create, reade, update, destroy)
 - ACID: Properties of a transactional database that guarantee data validity, even in the face of disaster recovery 
 (atomic, consistent, isolated, durabe) 
 - CAP Theorem: Three desirable attributes of a distributed database. You can have, at most, two of three (consistent, available, partition intolerance)
 - First normal form: Cells in a database contain one atomic item (e.g. not lists or sets)
 - Second normal form: No variable is wholly determined by other variables (no redundant columns)
 - Third normal form: No variable is indirectly determined by other variables (all information serves to describe the foreign key, and nothing else)
 
### Distributed systems

 - MapReduce: An architecture for efficiently processing large distributed data sets in a parallel
 - Directed acyclic graph: A paradigm for defining a program as a series of atomic steps, and the chain between those 
 steps
 - Sharding: Distributing data across multiple physical machines
 - Compute to data: It is often easier to move small code files to large amounts of data, rather than move large 
 amounts of data to small code files
 - Dealing with hardware failures
 - Dealing with slow communication / dropped messages

### Data structures & algorithms

 - LinkedLists
 - Heaps 
 - Stacks & Queues
 - Graphs
 - Binary search trees
 - Binary search
 - Sorting algorithms
   - Merge sort
   - Quick sort (pivot sort)
   - Bubble sort
   - Selection sort
   - Shuffle sort
      
### Project management

 - Agile: A project management framework emphasizing collaborative and ongoing project scoping and development
 - SCRUM: A project management framework designed to streamline project management, through pre-defined roles and
  meetings
 - Kanban: A lean project management framework, emphasizing visual process management and balancing capacity and demands
 - Waterfall: A project management framework which emphasizes working linearly through a set of pre-defined phases

## Soft skills

Tech as a whole, and data science in particular, have identified the 'genius asshole' trope as a nemesis to 
progress, and are putting a lot of effort into making sure that candidates play well with others. It's an easy fight to 
get behind.

While interviewing you, folks want to know if you a good person to be around, and someone they'd like to work with. Let 
your true self shine through, and let them know how awesome your are.   

 - STAR method: Describing a project or situation from an individual's point of view, emphasizing the situation, task, 
 action and resul
 - Building trust w/ colleagues / direct reports
 - Disagreeing w/ colleagues / direct reports
 - What are you looking for next?


