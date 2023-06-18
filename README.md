# Pine Tree Chatbot- AI-VR challenges 1.
[Colab notebook ]([url](https://colab.research.google.com/drive/1qHHpsrRqTQcwcwqIwp3raPqUpFOFJrwm?usp=sharing))

## Introduction
This is a simple rule-based chatbot built in Python that provides information about pine trees. It leverages Natural Language Processing (NLP) using the sentence transformer to understand and respond to user queries.

## Architect
I have collected question and answer pair of pine trees and used the sentence transformer model to convert the text of the question into sentence embedding. Now after embedding any query asked by the user, it finds the most similar questions related to the query using cosine similarity and returns the answer for the most similar question. Before providing the answer it checks if there is at least 70 % similarity with the question or not.


## Setup
1. Ensure you have Python 3.7 or later installed. You can check your Python version by running `python --version` in your terminal.
2. Install the required libraries like pandas, numpy, re, sklearn, and sentence transformer. For the sentence transformer install it by running `pip install sentence-transformers`

## Running the Chatbot
To start a conversation with the chatbot, run the notebook file. You can ask the chatbot questions about pine trees. If the chatbot doesn't know the answer to your question, it will let you know!

## Example Conversations
Here are some example questions you can ask the chatbot:

- What is a pine tree?
- How tall can a pine tree grow?
- What is the lifespan of a pine tree?
- Are pine trees evergreen?
- What are the uses of pine wood?
- What are pinecones?
- Where do pine trees grow best?
- How fast do pine trees grow?
- Do pine trees need a lot of sunlight?
- Can pine trees survive in the cold?
- Tell me about different species of pine trees.
- What is special about the bark of pine trees?
- Are pine trees good for the environment?
- Why are pine needles acidic?
- How does a pine tree reproduce?
- Why do pine trees have cones?
- How can I identify a pine tree?
- Can pine trees be used for medicinal purposes?
- What do pine trees symbolize?
- Do pine trees lose their needles?

## Extending the Chatbot
The knowledge of the chatbot is defined in a CSV in the `pine-data.csv` script, in the form of question-answer pairs. If you want the chatbot to know more about pine trees (or any other topic), you can extend this dictionary with more pairs.

## Limitations
This is a simple rule-based chatbot. It does not understand the context and cannot handle complex sentences or language nuances very well. To build a more complex model we can use models like BERT or GPT to finetune in the context of any specific tree. 
