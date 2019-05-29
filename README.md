# Dynamic-Lexicon-Generation-for-Natural-Scene-Images

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
<img src="pic1.jpeg" width="400" height="300">
<img src="re1.jpeg" width="400" height="300">
We can see the lexicon and their probabilties. To see more result open the final_cnn_inception_last_output.ipynb file.



#### Here is the link for the presentation on prezi
https://prezi.com/view/vvklNORa4kEiHcX3lA5z/





