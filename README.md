# Dynamic-Lexicon-Generation-for-Natural-Scene-Images

Introduction
----
Many scene text understanding  methods take huge benefit from using small per-image lexicons. Such customized lexicons are normally assumed as given and their source is rarely discussed.In this project we propose a method that generates contextualized lexicons for scene images using only visual information. 
Generates Contextualized lexicons based on visual information.We exploit the co-relation between the textual and visual information.Using the topic modeling framework to discover a set of latent topics in a dataset.We train a CNN model which is able to re-rank the words but using only the image raw pixels as input.

Dependencies
-----
1. gensim library
2. keras 
3. pickle 

### Reference of ResearchPaper
https://github.com/vishalbidawatka/Dynamic-Lexicon-Generation-for-Natural-Scene-Images/blob/master/PGR2016.pdf

##### Firstly ,we will suggest you to go through the research paper

How to Run
----
1. First you should download the dataset from MS-COCO site and links is given in data.txt
2. Change the path appropriately, and read the data.
3. First you have to run the LDA -> data.ipynb(Final LDA model), it will produce the two output file 
    *  first file have P(topic/document) in dictionary form   --> it will used as class label to train CNN model.
    *  second file have P(word/topic)    ---> with help of this, we will able to calculate the Probabilty (word/image).
4. CNN model ouput gives us the Probabilty(topic/image) just from the raw pixels without the textual information.



#### If you don't want to train the model
We already dump the model object , you can read the model object and run the code.

#### Result
<img src="1.png" width="700" height="400">
<img src="download (1).png" width="700" height="400">




#### Here is the link for the presentation on prezi
https://prezi.com/view/vvklNORa4kEiHcX3lA5z/





