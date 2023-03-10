# Text-Classification-using-BERT
the text classification model using the pre-trained BERT model
the text classification model using the pre-trained
BERT model, we are loading a train and test dataset, preprocesses the text data,
encodes the text data using BERT, and builds a model to predict the category of each
text. The pre-trained BERT model is used to encode the text data, and a neural network
is used as the classifier, we are using the TensorFlow library and predicting the
classification.
Here I have used a train and test dataset which had 1,20,000 text and 4 labels

![image](https://user-images.githubusercontent.com/110291143/224363093-b626f862-ed11-4c21-a3bc-ee7acb254b08.png)

And for each label there was 30,000 text

![image](https://user-images.githubusercontent.com/110291143/224363510-0273a3dc-9c27-4571-a0a4-2608e404452c.png)


1= "World"
2 = "Sports"
3 = "Business"
4 = "Sci/Tech"

And to make my model training easy and also as mention in the assignment “i have to
take a dataset of minimum of 1,000 each for label” i reduced my dataset for 2,000 for
each label so at present i trained the model with total of 8,000 line

![image](https://user-images.githubusercontent.com/110291143/224363637-d2cfef9c-fedc-4add-bd3e-daa5a32e55bb.png)

![image](https://user-images.githubusercontent.com/110291143/224363660-44f86d3a-7a13-43ab-9f63-a57a1ba5810e.png)

At start there were 3 column in the dataset names [class Index, Title, Description]
The Title and Description is merged to a single column names Text and Class Index
column name is renamed into Label

And for Visulaizing the categories i have named the label for there respective label

![image](https://user-images.githubusercontent.com/110291143/224363748-01ca721b-9af4-4a88-abab-f46373756500.png)

PreProcessing: The Preprocessing is done by removing all the stopwords, removing all
the special characters and converting the alpheberts into lower case and created a new
column named clean_text and saved the preprocessed data under it.
Architecture: This this Assignment i have used BERT base Model.
BERT base model has 12 layers (transformer blocks), 12 attention heads, and 110
million parameters

![image](https://user-images.githubusercontent.com/110291143/224363849-122c9338-c48a-4899-9cf9-8381afcdf56e.png)


Evaluation:

![image](https://user-images.githubusercontent.com/110291143/224363907-4e9de0dd-9c11-47f8-88f3-9a5b17adce6a.png)

We can improve the accuracy by using a larger dataset has here i have used a small
dataset. We can fine tune the BERT mode with different pre-processing techniques.
Sample Prediction:

text = ["Reuters - A car bomb exploded near a U.S.\military patrol in the
town of Baiji, north of Baghdad, on\Tuesday, killing at least seven Iraqis
and wounding 20 people,\including two U.S. soldiers, doctors and the
military said."]

![image](https://user-images.githubusercontent.com/110291143/224364031-0395b575-665d-420b-a696-c9da3698fe18.png)
