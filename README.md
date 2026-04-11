# Summarize Text

This is one of the application of NLP and GenAI.

This is a application which generate text summary for the text dialogue .

In this we use a pre trained transformer model T5 (Encoder Decoder transformer) from hugging face transformer used T5 because it deals with text .Text as input and generate text as output and for faster training we have use T5-small (version) .

Also T5 (Text-to-Text transfer Transformer) is a encoder-decoder architecture it uses both components it follow a "Text-to-Text" framework where NLP task like translation , summarization are performed 

# STEP TO FINE TUNE OUR MODEL:

step 1: Before generating output we have to perform pre-processing for the input text like cleaning ,converting to Tokenid.

step2: For TokenIds in our T5 model we have pre-trained tokenizer we use it to convert our input to tokenids after tokenization we have "Token_ids" for each tokens generated and also have "Attention mask" respect to each tokenid which describe which tokenid is valid or invalid

step3:Load the model and assign the device 

step4:Then define the TrainingArguments and also the trainer(model) 

step5:Finally Train the model

Then save the model and used it for every summary generation .

# STEPS  EVERY SUMMARIZATION FOLLOWS:
step1: clean input data

step2: Tokenize the data with tokenizer of T5 

step3: Input the Toekns to the Model to generate the summary

step4: Decode the summary_Token_id  with the Tokenizer to text

We have also deployed this model using FASTAPI (python based web frame work).

FASTAPI buid a API end at the server side we have UVICORN as our web server (UVICORN is a light weight web server generally used with FASTAPI)
