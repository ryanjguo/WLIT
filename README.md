# WLIT - What Language Is This?

WLIT is a beginner hackathon project created to detect what language a given input is written in, using artificial intelligence. 
The languages that it can currently detect are English, French, Spanish, Portuguese, Italian, German, Swedish, Danish, Dutch, Russian, and Greek. 
The languages it can currently detect are limited by the dataset we used, as well as the modules we implemented. 

To read and manipulate our data, we used the _pandas_ module. To filter out unwanted characters, we employed the _re_ module. We used the spaCy module, that provides us with information about each language, such as the stopwords, lemmatization, and punctuation. Using the spaCy modules, we removed any punctuation and stopwords ("the", "a"), as well as lemmatized ("is" -> "be", "going" -> "go") each word. After finishing pre-processing, we used _sklearn_ to convert individual words into a vector counterpart. We further used _sklearn_ to identify which language our input is written in. Overall, the project was coded using Python on Google Colabs.

In the future, we hope to expand to more languages, with better accuracy with implementations such as detecting spelling errors. 
