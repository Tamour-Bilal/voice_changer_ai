# Voice_Changer_AI
The repo contains code for voice changer. It will be containing the testing as well as production level code. 
# Purpose of the APP 
Input string- maximum of 250 characters will be passed on the changeover app. THe app will then convert the text into speech. THe speech should be non robotic and resembling to human voice or speech. It should leverage text to speech model that have the emotions, punctuaution control.
# Certain limitations
1- Donot use prepaid services such as open ai, llm models etc.  
2- Prefer models that use less GPU storage 16gb or more is fine till now. 
# Initial RND and Selected Model. 
Many state of the art models are present that are multilingual and make conversions of text in voice, making use of different languages, however they have limitation of natural voice. Thier results resembles the robotic sounds. however Bark from suno ai has the voices that resembles more to the human and contains different emotions as well 
# Languages Support by Bark 
Languages Support by bark
    ("English", "en"),
    ("German", "de"),
    ("Spanish", "es"),
    ("French", "fr"),
    ("Hindi", "hi"),
    ("Italian", "it"),
    ("Japanese", "ja"),
    ("Korean", "ko"),
    ("Polish", "pl"),
    ("Portuguese", "pt"),
    ("Russian", "ru"),
    ("Turkish", "tr"),
    ("Chinese", "zh")

# Speakers 
It has support to the 100 speakers. Each language has many speakers but
# Model architecture and usage of resources. 
Model is consisted of three main models that works together to produce the output. 
At 8gb GPU, large models are unable to download, however small models can be downloaded and loaded. 

GPU usage is 12-13 gb for larger models, however small models can be loaded at 8gb as well. 
Optimization can be 
1- Offloading the models from gpu to cpu- once they have completed the processig. This can be achieved using the accelerate.


# Branches
Right now main branch is empty and it will contains the production ready code in future
There will be total three branches dev, prod and uat. 
dev branch will contains testing scripts and devlopment of api.
uat branch will contain uat or user testing i.e QA 
prod branch will be protected in future
# Testing of the API
1- The test sets have been prepared for all the languages covering support for emotions such as happy, sad, shouting and modifiers such as [laugh], [sighs] etc.


