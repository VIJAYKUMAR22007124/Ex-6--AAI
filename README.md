<H3>B VIJAY KUMAR</H3>
<H3>212222230173</H3>
<H3>EX. NO.6</H3>
<H3>DATE:23-04-2024</H3>
<H1 ALIGN =CENTER>Implementation of Semantic ANalysis</H1>
<H3>Aim: to perform Parts of speech identification and Synonym using Natural Language Processing (NLP) techniques. </H3> 
 <BR>
<h3>Algorithm:</h3>
Step 1: Import the nltk library.<br>
Step 2: Download the 'punkt', 'wordnet', and 'averaged_perceptron_tagger' resources.<br>
Step 3:Accept user input for the text.<br>
Step 4:Tokenize the input text into words using the word_tokenize function.<br>
Step 5:Iterate through each word in the tokenized text.<br>
•	Perform part-of-speech tagging on the tokenized words using nltk.pos_tag.<br>
•	Print each word along with its corresponding part-of-speech tag.<br>
•	For each verb , iterate through its synsets (sets of synonyms) using wordnet.synsets(word).<br>
•	Extract synonyms and antonyms using lemma.name() and lemma.antonyms()[0].name() respectively.<br>
•	Print the unique sets of synonyms and antonyms.
<H3>Program:</H3>

#### Install NLTK using pip

```
!pip install nltk
```

#### Import necessary NLTK modules

```
import nltk
from nltk.tokenize import word_tokenize
```

#### Download NLTK resources

```
nltk.download('punkt')
nltk.download('averaged_perceptron_tagger')
nltk.download('wordnet')
```

#### Get user input sentence

```
sentence = input()
```

#### Tokenize the sentence into words and Perform part-of-speech tagging

```
words = word_tokenize(sentence)
pos_tags = nltk.pos_tag(words)

```

#### Print words with their corresponding part-of-speech tags

```
for word, tag in pos_tags:
    print(word, tag)
```

#### Identifying synonyms and antonyms of each word

```
for word in words:
	for syn in wn.synsets(word) :
		for lemma in syn.lemmas():
			synonyms . append (lemma . name( ) )
			if lemma . antonyms():
				antonyms . append ( lemma. antonyms ( ) [0] . name ( ) )
```

#### Print the sets of synonyms and antonyms

```
print ( "Synonyms : " ,set (synonyms) )
print ( "Antonyms : " ,set(antonyms) )
```

<H3>Output</H3>

##### INPUT -> "Harish is a Human Being"

 ![image](https://github.com/VIJAYKUMAR22007124/Ex-6--AAI/assets/119657657/73c71ddc-468f-4f69-9d01-8d1fc9ec02dc)

##### Synonyms and Antonyms

![image](https://github.com/VIJAYKUMAR22007124/Ex-6--AAI/assets/119657657/9e68245f-3bb3-4556-8707-10d3576f1892)



<H3>Result:</H3>
Thus ,the program to perform the Parts of Speech identification and Synonymis executed sucessfully.
