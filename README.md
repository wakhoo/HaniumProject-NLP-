# Hanium LDA

### Intro

This project is about **Analysis of semantic-based technical documents (paper/patent) using artificial intelligence**

When searching for a thesis or patent document (hereafter referred to as a technical document) or creating a new technical document, the user can **find the desired technical document with key keywords and topics** based on them.

By analyzing technical documents using artificial intelligence, key keywords and topics are presented, and key keywords are visualized and presented to users.


### Schematic Diagram

<img src="https://github.com/wakhoo/HaniumProject-NLP-/blob/main/resourse/hanium_schematic_diagram.png?raw=true">


### Demo Video
<a href="https://youtu.be/cBynl_P0z6M"><text>Link to YouTube</text></a>

### Result

#### NLP

<img src ="https://github.com/wakhoo/HaniumProject-NLP-/blob/main/resourse/ppt/%E1%84%92%E1%85%A1%E1%86%AB%E1%84%8B%E1%85%B5%E1%84%8B%E1%85%B3%E1%86%B7LDA.015.png?raw=true">

<br><br>

- We export Lemma by using WordNetLemmatizer provided by NLTK.
- Exporting Lemmatization is the process of finding a Lemma from words.
    - For examples 'am', 'are', and 'is' are different spellings, but we can see there root word as 'be'. Like this we called 'be' is the Lemma of those words.
- Unlike stemming, Lemmatization shows a pattern in which the form of words is appropriately preserved

---
#### TF-IDF

<img src ="https://github.com/wakhoo/HaniumProject-NLP-/blob/main/resourse/ppt/%E1%84%92%E1%85%A1%E1%86%AB%E1%84%8B%E1%85%B5%E1%84%8B%E1%85%B3%E1%86%B7LDA.016.png?raw=true">

<br><br>

- Use the TfidfVectorizer provided by scikit-learn.
- The TF-IDF weighting matrix is a method of weighting the importance of each word using the frequency of the word and the frequency of the reverse document.
- If the value is small, the importance is low, and if it is large, the importance is high.
- Words that frequently appear in all documents are judged to be of low importance, and words that frequently appear only in certain documents are judged to be of high importance.


---
#### LDA

<img src="https://github.com/wakhoo/HaniumProject-NLP-/blob/main/resourse/ppt/%E1%84%92%E1%85%A1%E1%86%AB%E1%84%8B%E1%85%B5%E1%84%8B%E1%85%B3%E1%86%B7LDA.017.png?raw=true">

<br><br>

- Fifteen topics of science and technology research are presented in Table 1 along with related words.
- Topic is numbered in descending order of proportion.
- We proceed Top 15 topic labeling
- It shows research themes in specific fields related to science and technology research.

<img src="https://github.com/wakhoo/HaniumProject-NLP-/blob/main/resourse/ppt/%E1%84%92%E1%85%A1%E1%86%AB%E1%84%8B%E1%85%B5%E1%84%8B%E1%85%B3%E1%86%B7LDA.018.png?raw=true">

<br><br>


- In Figure 1, a relatively large circle represents a topic with a high frequency in corpus.
- The topic is more similar when each circle is closer,  the more different the topic is when each circle is farther.
- When a circle is selected, the representative words and frequencies of the topic are show as graphs on the right side.

<br><br>

Reference
- https://wikidocs.net/book/2155
- 그림 2, LDA 토픽 모델링의 이해, Probabilistic topic models, DaviD m. Blei 2012.04)
