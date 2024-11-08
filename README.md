# -*- coding: utf-8 -*-
"""_Translation_nlp_application.ipynb

Automatically generated by Colab.

Original file is located at
    https://colab.research.google.com/drive/1T8LEopk57QItWn1ZKfhyBlFSFMeyfNuf
"""

# Install the 'transformers' library, which provides pre-trained NLP models
!pip install transformers

# Install the 'transformers' library with additional support for sentencepiece,
# which is used for tokenization in some models (like multilingual models)
!pip install transformers[sentencepiece]

# Import the 'pipeline' function from the 'transformers' library
from transformers import pipeline

# Initialize a translation pipeline for English to Italian using a pre-trained model
# The model 'Helsinki-NLP/opus-mt-en-it' is specifically trained for this language translation
text_translator = pipeline("translation_en_to_it", model="Helsinki-NLP/opus-mt-en-it")

# Install the 'transformers' library with additional support for sentencepiece,
# which is used for tokenization in some models (like multilingual models)
!pip install transformers[sentencepiece]

# Define the English text that you want to translate to Italian
input_text = "This text is translated from English to Italian"

# Use the translation pipeline to translate the English text to Italian
# 'clean_up_tokenization_spaces=True' removes extra spaces in the output
italian_text = text_translator(input_text, clean_up_tokenization_spaces=True)

# Print the translated text in Italian
print(italian_text)

# Import the 'pipeline' function again (this is redundant but does not cause issues)
from transformers import pipeline

# Initialize another translation pipeline for English to Urdu using a pre-trained model
# The model 'Helsinki-NLP/opus-mt-en-ur' is used for English to Urdu translation
text_translator = pipeline("translation_en_to_ur", model="Helsinki-NLP/opus-mt-en-ur")

# Define the English text that you want to translate to Urdu
urdu_input_text = "This text is translated from English to urdu"

# Use the translation pipeline to translate the English text to Urdu
# 'clean_up_tokenization_spaces=True' ensures the output is formatted cleanly
urdu_text = text_translator(urdu_input_text, clean_up_tokenization_spaces=True)



# Import the 'pipeline' function again (this is redundant but does not cause issues)
from transformers import pipeline

# Print the translated text in Urdu
print(urdu_text)

# Initialize another translation pipeline for English to German using a pre-trained model
# The model 'Helsinki-NLP/opus-mt-en-ur' is used for English to Germen translation
text_translator = pipeline("translation_en_to_de", model="Helsinki-NLP/opus-mt-en-de")

# Define the English text that you want to translate to Urdu
German_input_text = "This text is translated from English to German"

# Use the translation pipeline to translate the English text to Urdu
# 'clean_up_tokenization_spaces=True' ensures the output is formatted cleanly
German_text = text_translator(German_input_text, clean_up_tokenization_spaces=True)

# Print the translated text in Urdu
print( German_text)

# Initialize another translation pipeline for English to German using a pre-trained model
# The model 'Helsinki-NLP/opus-mt-en-ur' is used for English to Germen translation
text_translator = pipeline("translation_en_to_fr", model="Helsinki-NLP/opus-mt-en-fr")

# Define the English text that you want to translate to Urdu
French_input_text = "This text is translated from English to French"

# Use the translation pipeline to translate the English text to French
# 'clean_up_tokenization_spaces=True' ensures the output is formatted cleanly
French_text = text_translator(French_input_text, clean_up_tokenization_spaces=True)

# Print the translated text in French
print( French_text)

# Initialize another translation pipeline for English to German using a pre-trained model
# The model 'Helsinki-NLP/opus-mt-en-ur' is used for English to Germen translation
text_translator = pipeline("translation_en_to_es", model="Helsinki-NLP/opus-mt-en-es")

# Define the English text that you want to translate to Spanish
Spanish_input_text = "This text is translated from English to Spanish"

# Use the translation pipeline to translate the English text to Spanish
# 'clean_up_tokenization_spaces=True' ensures the output is formatted cleanly
Spanish_text = text_translator(Spanish_input_text, clean_up_tokenization_spaces=True)

# Print the translated text in French
print( Spanish_text)

# Initialize another translation pipeline for English to Japanese using a pre-trained model
# The model 'Helsinki-NLP/opus-mt-en-ur' is used for English to Japanese translation
text_translator = pipeline("translation_en_to_jap", model="Helsinki-NLP/opus-mt-en-jap")

# Define the English text that you want to translate to Japanese
Japanese_input_text = "This text is translated from English to Japanese"

# Use the translation pipeline to translate the English text to Japanese
# 'clean_up_tokenization_spaces=True' ensures the output is formatted cleanly
Japanese_text = text_translator(Japanese_input_text, clean_up_tokenization_spaces=True)

# Print the translated text in Japanese
print( Japanese_text)

