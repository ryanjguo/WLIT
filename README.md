# WLIT - What Language Is This?
<h5>Authors:</h5>
<b>Ethan Huynh, Sahitya Nulu, Ryan Guo, Roshan Dewmima</b>
<h5>What is WLIT?</h5>
<p>WLIT is a beginner hackathon project created to detect what language a given input is written in, using artificial intelligence. 
The languages that it can currently detect are English, French, Spanish, Portuguese, Italian, German, Swedish, Danish, Dutch, Russian, and Greek. 
The languages it can currently detect are limited by the dataset we used, as well as the modules we implemented. </p> 

A video demo of the product can be seen [here](https://youtu.be/KSlAkXiAuDY)

<h5>Dataset</h5>
<p>The <a href = https://www.kaggle.com/datasets/basilb2s/language-detection>dataset</a> that we chose for this project is the language detection dataset by Basil Saji from Kaggle. According to Basil he "Collected the data from Wikipedia by scraping using BeautifulSoup python library".</p>

<h5>Methodology</h5>
<p>To read and manipulate our data, we used the _pandas_ module. To filter out any unwanted characters, we employed the _re_ module. We used the spaCy module, that provides us with information about each language, such as the stopwords, lemmatization, and punctuation. Using the spaCy modules, we removed any punctuation and stopwords ("the", "a"), as well as lemmatized ("is" -> "be", "going" -> "go") each word. After finishing pre-processing, we used _sklearn_ to convert individual words into a vector counterpart. We further used _sklearn_ to identify which language our input is written in. Overall, the project was coded using Python on Google Colabs.</p>

In the future, we hope to expand to more languages, with better accuracy with implementations such as detecting spelling errors. 
