# Document-Classification-and-information-extraction-
#### NLP project which classifies PDF documents and extract information 

 ###### Business use case of this project
 
In a Law or Insurance companies we have lot of documents that are crucial for the work flow, like in law firms, case documents, user agreements in insurance firma. A major bottleneck in the Law firms is not getting the documents reviewed in time and not getting the Due Diligence done in time.

  To avoid this we can use this document classification and information extraction to split the large documents into small individual docs and extract the necessary information from them. This was proved to increase the productivity by 80% in a Law firm of USA, Stockwell.
  
 ###### Process
 I have built a Document classification and information extraction tool, in which I have trained a Machine Learning model to classify documents and based on the result class i will extract specific fields in the document using either Regex or text manipulation.
 I am taking both scanned or normal text PDFs to classify them.
 
 If I get any scanned PDF I am using PyTesseract (OCR: Optical Character Recognition) to get the text from the scanned image.
 
 If i am getting a text PDF them i am converting the PDF into a txt file.
 
 I will classify the documents based on the text that i am extracting above and based on the result class i will extract information from the same text
 
###### Model Building
I have used the Data available on the internet which is of classes, Agreements, Human Resources and Taxes.

First, i have preprocessed the data by removing, all “Punctuations”, “special characters”, “Line Breakers (/n)” and many more irrelevant information.

Then I am using TFIDF to vectorize the text.

I am using XG Boost to train the vectorized data.

I have tried other algorithms as well but XGBoost gave best results.

As you know XGBoost is a greedy algorithm and very efficient to train on data with very less variance among the classes. And It has a number of Parameters to tune and get the best results possible.

