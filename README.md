# Chatty
Chatty is a Python Langchain based application which takes a pdf file or files and it acts as a virtual assistant related to the file. You can ask questions related to the file and even prompt a task.
Chatty use the following Python frameworks:
1) Streamlit
2) Langchain
3) PyPDF2
4) Google_Gemini_Pro LLM
5) Google_Gemini_embeddings Algo
6) Pinecone

FUNCTIONALITY:
A) It first takes a pdf or group of pdf files
B) It divides it into Chunks
C) Then an embedder(Gemini Embedder in this case) converts the chunks into Vectors and places similar vectors together on the basis of Euclidean Distance.
D) We store the Vectors in Pinecone virtual database 
E) After all, it takes a user query and searches in the Vector Database.
F) Finally, results is displayed on Streamlit TextField.
