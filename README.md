# Fragabs
This is an AI-powered abstract analyzer that takes medical research paper abstracts as input and simplifies them by labeling sentences with OBJECTIVE, BACKGROUND, METHODS, RESULTS, and CONCLUSIONS.

To enhance the user experience, we developed a React-based frontend that integrates a dictionary feature. 

With just a double-click, users can look up the meaning of a word, saving them time from having to search for it elsewhere.

For the backend, we used Django, which provides caching features that we used to cache the ML model, resulting in a significantly faster runtime (about 4 times faster).

This machine learning model was built using the TensorFlow framework and NLP approach, and it was trained on over 200,000 samples of medical abstracts. 

To handle the massive dataset, we used deep learning techniques. 

We ran a series of experiments and used different model architectures, such as Dense, Conv1D, BiLSTM, Dense with Character Embeddings, and a Tribrid model using feature engineering.

Our hybrid model, consisting of a BERT pre-trained model and feature engineering, helped us achieve our highest accuracy, with 93% accuracy on the training data and 88% accuracy on the validation data.

# Steps to run the project
1. Install the front end dependencies using "npm install"
2. In the backend folder, activate the environment by going to the directory backend/fragabs/
3. Install the dependencies in the "requirements.txt" file using "pip install"
4. Start the front-end using "npm start" command
5. Start the backend using "python manage.py runserver" command
6. You are good to go
