# Political_analysis_and_hatespeech_detection_app

This is a political analysis and hatespeech detection application built using streamlit. 
It collects Twitter and Facebook data and analyzes it to identify the popularity of politicians and their political parties.

The first part involves collecting data from either Twitter or facebook.
To collect data from Facebook, find a post, paste the facebook mobile link into the text box and collect  all the comments from the post.
Ensure the link is from Facebook Mobile.

To collect data from Twitter, you can either post a Twitter post url or search for a topic and get tweets.
For collecting tweets for a topic, you are also required to specify the number of results collected.

The second part involves analyzing the tweets and Identifying the entities mentioned in the data collected. I trained a spacy model to identify politicians and Political parties from text and used it to identify entities mentioned in the data.

Analysis is then performed to identify the top 10 most mentioned entities, ie politicians and political parties. We then perform sentiment analysis for the top 3 mentioned politicians to identify whether the text mentioning them was positive, negative or neutral. Vader sentiment analysis was used for sentiment analysis.

The next part involved identifying the hatespeech text. A model was trained using supervised machine learning and a Naive Bayes Classifier to create a model that classified text as either hateful or not hateful.
The model was passed to the data and a chart of the distribution of data was created. 

All the libraries used are found in the requirements.txt file.

To run the app, ensure you have your own twitter API keys saved in a txt file. Clone the project to your repository and run the project using streamlit run command.
The main file is project.py
