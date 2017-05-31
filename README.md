# Initial insights from text

In this assignment, we'll be using what we learned from class to dissect an interesting data set.
We'll be looking at the Random Acts of Pizza Dataset, where Reddit users ask other Reddit users to send them pizza for free.
You can check out more information [here](https://cs.stanford.edu/~althoff/raop-dataset/).
We'll be applying different types of analyses to each pizza request, so make sure to define functions to complete the tasks.
That way, you can just call them on all the requests individually and collect the results in e.g. a list.

## Getting started

1. Read in the data using the starter notebook.
2. Each line in the file contains an individual request. Using SpaCy, parse each request *individually*, which is different from parsing the entire file like we did in class. You could start by breaking the requests into in a list, and parsing each element of the list.

## Initial insights

1. *n*-grams are groups of consecutive words. Identify all of the unique unigrams (single words), bigrams (two words), and trigrams (three words) that appear across all of the requests. Report how many unique unigrams, bigrams, and trigrams there are.
2. Find the trigram that appears in the highest number of requests.
3. Using the dependency tree and part-of-speech tags, identify the adjective and verb that describe the word `pizza` most frequently.

## Going deeper

1. Get the GloVe embedding for `pizza` and find the most similar word in the corpus by cosine distance
2. Look up TF-IDF (term-freqency inverse-document-frequency) on the world wide web. Using each request as a document, find the 10 unigrams with the highest TF-IDF and the 10 words with the lowest TF-IDF in the document. Do the same for bigrams. Don't try to use a library for this task. You should be able to compute it using NumPy without too much trouble.

## Coming up with your own analysis

Come up with three original insights similar to the previous ones.
Make sure they're interesting!
At least one needs a plot, and at least one needs to have a downstream analysis with a conclusion.
For example, you might want to find the cities that occur most frequently so that you use this data to upsell online adds to pizzerias in these cities (but now you can't do this one because I did it).
**Spend 30-45 minutes per insight.**
