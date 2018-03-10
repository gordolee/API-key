### API-key
## How to use an API Key


Your API key is your ticket to extracting information from an API. It is not something that you should share with other people, since your account could be compromised and sensitive information would be leaked. Instead, you should host the key in a separate environment, not embedded in the code that you will upload.

Other good practices include deleting unused API keys, and periodically regenerating your keys.

A common way to utilize an API Key is to create a separate file (e.g. keys.R) where you define a key through a variable, such as API_KEY. This file would be saved locally, but added to a .gitignore directory so that it does not get shared like the rest of the repository. That way, your information would be secure. 

To access keys.R, you can utilize R's very useful and handy "source" function, which allows your to source a different file to use the contents of said file, allowing you to use the predefined variables (including API_KEY) in your main code. By calling the variable instead of typing the actaul API key, you are maintaining a safe practice of keeping the private information of your API private.
