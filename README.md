# Summarize Text

This is one of the application of NLP.

This is a application which generate text summary  of the text dialogue .

In this we use a pre trained transformer model T5 from hugging face transformer used T5 because it deals with text take text as input and generate text as output and for faster training we have use T5-small version .

Also T5 (Text-to-Text transfer Transformer) is a encoder-decoder architecture it uses both components it follow a "Text-to-Text" framework where NLP task like translation , summarization are performed 

In this we need to perform pre-processing of the input text .

We have fin tune the model on our own dataset to train the model for a specific task i.e text summary.

Then save the model and used it for every summary generation .

We have also deployed this model using FASTAPI (python based web frame work).

FASTAPI buid a API end at the server side we have UVICORN as our web server (UVICORN is a light weight web server generally used with FASTAPI)
