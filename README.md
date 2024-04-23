# CSE508_Winter2024_A4_23064
Data loading:- 
->loaded dataset from the csv using pandas 
->printed its shape to understand its dimensions 
->checked the missing values and dropped missing values 
Text Preprocessing:- 
->created copy of original dataframe to preserve the preprocessed data separately 
->converted text data to lowercase to ensure consistency 
->removed special characters 
->applied tokenization using nltk’s word_tokeinze function 
->removed stop words from the text using nltk’s stopwords corpus 
->lemmatized the text to convert words to their base form using nltk’s WordNetLemmatizer 
Model Training:-
, I have first initialised the gpt2 tokenizer and gpt2 model from hugging face 
->then I created custom dataset class to format data fro training 
->spilit the dataset into training and testing sets of 75:25 ratio 
->defined batch size, data loaders , optimizer , scheduler and no of epochs for training our model 
->trained the gpt2 model using the training dataset and fine tuned it for review summarization 
->utilized the adamW optimizer and implemented training loops, also checked for empty tensors and 
handled exceptions also 
->saved the fine tuned model for future use.
Evaluation:-
>evaluated the gpt2-model’s performance for generating summaries for review text using rough 
metrics 
->calculated rouge scores(rough-1,rough-2,rough-L) for evaluation 
Results:- 
->provided a sample text and given the actual summary or ground truth summary 
->obtained generated summary from the gpt2 model 
->calculated rough scores-precision,recall and f1 scores. 
