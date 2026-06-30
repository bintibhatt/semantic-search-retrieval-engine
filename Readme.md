# Semantic Search & Retrieval Engine

## Overview

The Semantic Search & Retrieval Engine offers three distinct search options:

- Basic Search functionality in this identifies sentences that directly contain the exact form of specified keywords, without any lemmatization applied. This search method is effective for precise matches based on the literal appearance of keywords in the text.

- Root Word Search employs lemmatization to match sentences based on the root forms of the provided keywords. This approach allows for a more comprehensive search, capturing variations of the keywords and enhancing the scope of relevant results.

- Context Search leverages BERT embeddings, a state-of-the-art natural language processing technique. By assessing contextual similarity, this search option identifies sentences that contextually align with the input keywords, offering a nuanced and semantic understanding of the text. This method is particularly useful for uncovering sentences with similar meanings or themes.

## SetUp

1. Open the directory.
2. Install libraries: `pip install requirements.txt`
3. Run: ` python your_app_name.py`
4. By running run_app.py, it will download:

- nltk.download('punkt')
- nltk.download('averaged_perceptron_tagger')
- nltk.download('wordnet')

5. Open http://127.0.0.1:5000 on a browser.

## How to test ?

- Open TestCases Folder
- Use any test cases present in the folder.
- Add the paragraph in first input box and the keywords only in the second input box.
- Select what type of search you want to perform from the options: Basic, Root, Context
