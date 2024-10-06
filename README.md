# Gemini Health App
**Project Overview**

This project demonstrates a health management application utilizing Google's Generative AI technology (Gemini).  The app focuses on analyzing user-uploaded images of food items and estimating total calorie content.

**Technologies Used**

_Streamlit:_ A Python library for creating interactive web applications.<br>
_dotenv:_ A Python library for loading environment variables from a .env file.<br>
_google.generativeai (GenAI):_ Google's API for accessing Generative AI models, including Gemini.<br>
_PIL (Python Imaging Library):_ Provides image processing functionalities.<br>
Requirements

Python environment with required libraries installed (Streamlit, dotenv, GenAI, PIL).<br>
Google Cloud Project and API key for GenAI access.<br>
A pre-trained Gemini model configured for image analysis and text generation ("gemini-pro-vision").<br>

**How it Works**<br>

_User Interface (UI):_<br>
The app starts with a title and input prompt field for users to specify additional information.<br>
Users can upload an image containing food items.<br>
A submit button triggers the analysis.<br>
_Image Processing:_<br>
Upon submission, the uploaded image is converted into a format suitable for the Gemini model.<br>
_GenAI Integration:_<br>
The pre-defined input text instructs the model to analyze the image and identify food items, then calculate the total calorie content.<br>
The GenAI model processes the user prompt, image data, and predefined text to generate a response.<br>

_**Output:**_<br>
The app displays the generated response, potentially listing identified food items and their estimated calorie intake.<br>

**Key Code Snippets**

_get_gemini_response() function:_

![image](https://github.com/user-attachments/assets/c4328db9-531b-440b-9718-4d3b87fed0bb)

_input_image_setup() function:_

![image](https://github.com/user-attachments/assets/fbf91a4d-50ed-4552-bada-6bcf315733b7)

_**Main application logic:**_

![image](https://github.com/user-attachments/assets/aa16e4f2-198b-48f3-becc-cb108b84cd21)


_**Limitations**_

_Accuracy:_ The calorie estimations provided are based on the model's training data and may not be perfectly accurate for every image.<br>
_Model Specificity:_ The current implementation uses a generic "gemini-pro-vision" model. Training a custom model specifically for food image analysis might improve accuracy.<br>
_Limited Functionality:_ This is a basic example, and the app could be expanded to offer additional features like dietary recommendations or personalized advice.<br>

**Future Improvements**

Integrate with a calorie database for more accurate estimations.<br>
Allow users to specify dietary restrictions.<br>
Enhance the UI to display identified food items within the image.<br>
Train a custom model specifically for food image analysis and calorie estimation.<br>
Overall, this project showcases the potential application of Generative AI in health management. By leveraging image recognition and language generation, such tools can offer users a convenient and informative way to keep track of their dietary intake.<br>

