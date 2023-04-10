# Voice-chatGPT
### simple chatbot that uses speech recognition, text-to-speech conversion, and OpenAI's natural language processing
This code is an example of a simple chatbot that uses speech recognition, text-to-speech conversion, and OpenAI's natural language processing capabilities to carry on a conversation with a user. The chatbot is designed to respond to spoken inputs from the user using a microphone, and generate text responses using OpenAI's text generation capabilities.

Here's how the code works:

    1) The script starts by importing the necessary libraries: speech_recognition for speech recognition, pyttsx3 for text-to-speech conversion, and openai for natural language processing.

    2) The OpenAI API key is set using openai.api_key.

    3) The pyttsx3 engine is initialized, and the desired voice is selected using engine.setProperty.

    4) A Recognizer object is created from the speech_recognition library, and a Microphone object is created to capture audio input.

    5) The conversation variable is initialized to an empty string, and the names of the user and bot are set to "Dan" and "John", respectively.

    6) The main loop of the chatbot starts, which continues indefinitely until the user stops the script. Within the loop, the chatbot waits for audio input from the user using the microphone.

    7) The audio input is transcribed to text using Google's speech recognition API, and the resulting text is stored in the user_input variable.

    8) The prompt variable is created by concatenating the user_name, user_input, and bot_name strings. This prompt is used as input to the OpenAI API to generate the bot's response.

    9) The OpenAI API is called with the prompt variable and some additional parameters, such as the model to use, the maximum number of tokens to generate, and the temperature parameter that controls the randomness of the generated text.

    10) The bot's response is extracted from the OpenAI API's response, cleaned up to remove any extraneous text, and added to the conversation variable.

    11) The bot's response is spoken aloud using the pyttsx3 library's say and runAndWait functions.

    12) The loop continues, waiting for the next audio input from the user.

Overall, this code demonstrates the power of combining speech recognition, text-to-speech conversion, and natural language processing to create a simple but effective chatbot that can converse with a user using spoken language.
