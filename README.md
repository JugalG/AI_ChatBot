# AI ChatBot

This project is an AI chatbot that uses NLTK, TFlearn, TensorFlow, and deep learning techniques to respond to user input based on predefined intent patterns and responses. The chatbot is designed to engage in text-based conversations and provide relevant answers to user queries.

![ChatBot](chatbot.jpg)

## Python and Library Versions

The chatbot was developed using the following specific library versions:

- Python: 3.6.0
- NLTK: 3.6.7
- NumPy: 1.16.6
- TFlearn: 0.3.2
- TensorFlow: 1.15.0

Please make sure you have these exact library versions installed to ensure compatibility with the code.

## Credits

This chatbot project is inspired by the tutorial created by Tech With Tim. You can find the tutorial on YouTube or the website for step-by-step guidance on building your chatbot:

- [YouTube Tutorial Playlist](https://youtube.com/playlist?list=PLzMcBGfZo4-ndH9FoC4YWHGXG5RZekt-Q&si=kyOlRclkPpJPZCo5)
- [Website Tutorial Guide](https://www.techwithtim.net/tutorials/ai-chatbot/part-1)

## Project Structure

Here's an overview of the project's structure and key components:

- `intents.json`: A JSON file that defines the intent patterns and responses used to train the chatbot. Each intent contains a tag, a list of patterns (user queries), and a list of responses (bot replies).

- `train_chatbot.py`: The script that preprocesses the data, trains the chatbot using deep learning techniques, and saves the model and data for future use. This script also loads the model if it already exists.

- `chatbot.py`: The script that handles user input and engages in a conversation with the chatbot. It loads the trained model and responds to user queries.

- `data.pickle`: A binary file that stores preprocessed training data (words, labels, training, and output).

- `model.tflearn`: The trained chatbot model saved in TFlearn format.

## How to Use the ChatBot

To use the chatbot, follow these steps:

1. Make sure you have the required Python and library versions installed.

2. Clone or download this repository to your local machine.

3. Run the `train_chatbot.py` script to preprocess data and train the chatbot. If the model and data files already exist, the script will load them.

4. Once training is complete, run the `chatbot.py` script to start a conversation with the chatbot.

5. Type your queries and interact with the chatbot. You can exit the conversation by typing "quit."

## Important Notes

- The chatbot's performance is based on the quality and quantity of training data in the `intents.json` file. You can extend and customize the intents to improve the chatbot's responses.

- The chatbot uses a confidence threshold of 0.7 to determine whether to respond to a query. If the confidence is below 0.7, it will display a message indicating that it didn't understand the query.

- Feel free to modify the code and expand the chatbot's capabilities, such as adding more intents, handling specific topics, or improving the user experience.

Enjoy chatting with your AI ChatBot!

For more details and guidance, refer to the provided tutorial links in the "Credits" section.
