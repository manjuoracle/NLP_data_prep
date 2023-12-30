om

basics------------------------------------------
#series is  a datatype in pandas , the other data type in pandas is DataFrames Note: pandas has only 2 type of Dtypes

#why we need to use .tolist() in passing columns as input because in DataFrames columns are of series type, hence need to convert then to list 

#args can only be passed inside function, method, classes()

#[] hard barckets are used only when elements have to be access through spefing index number inside list or index

#difference between loc and iloc is ,iloc using index of row and columns, loc using column heading
#with can be add conditional selection also with loc
df.loc[1,"C"]#it shows data in row-2 and column-C
df.iloc[1,2]#it shows data in row-2 and column-3
dff.index=["apple","orange","grape","banana"]#changing the value of indices
df.iloc[::-1,:]#twisted whole rows
df.iloc[:,::-1]#twisted whole columns

#word2vec= need "Gensim" library, it forms vectors of each word using a shallow neural network -we get vector at word level , includes neigbour as suggested in window of n number of left and right negbhour words (used when we need to compare word to word ) [q&A, similarity, next word prediction]

#tfidf= will create embedding at document level only, similar to bag of word ( term frequency) BUT will give you highest score to most unique words, its improvement over bag of words [topic modelling(ldm), classifiaction, doc similarity]

#bag of words= count vectorizer = will create embedding at document level only, each document can include any number of words passed in ONE cell/row [used in topic modelling(ldm), classifiaction, doc similarity]

#ngram= how many words to be taken togeather for analysis ( unigram= 1 word, bigram , 2 , trigram= 3 words etc.breaks the sentence in "n"gram for analysis)

#skip gram= #continuous bag of words are TWO methods of generating embeddings for word to vec models


For loop_______________________


# step1: create empty list to storage iterative values of each element
# step2: for ele in "name of the list from which elements have to be iter'ed"
# step3: empty_list.append("elements list have to be iter'ed ")
# step4: print to check empty list

#args can only be passed inside function, method, classes()
#[] hard barckets are used only when elements have to be access through spefing index number inside list or index


word2vec

#     Parameters:
#     doc_tokens   : A tokenized document
#     epochs       : Number of epochs training over the corpus
#     workers      : Number of processors (parallelization)
#     vector_size  : Dimensionality of word embeddings
#     window       : Context window for words during training

#     min_count    : Ignore words that appear less than this


DATA---------------------------
np.random.randint(0,100,20).reshape(4,5)

!wget https://cs.stanford.edu/people/alecmgo/trainingandtestdata.zip
!unzip /content/trainingandtestdata.zip
pd.read_parquet("/content/0000.parquet")
pd.read_excel("/content/PPI.xlsx", sheet_name='Sheet1')
 
 !pip install pdfminer.six
 from pdfminer.high_level import extract_text
doc1 = extract_text("/content/doc1.pdf")
print(doc1)
#HOW TO INPUT DATA to model
example = input("enter you question: ")
