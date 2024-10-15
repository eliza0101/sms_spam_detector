# sms_spam_detector
Module 21 Challenge


**Overview:**
This project implements an SMS spam classification system using machine learning techniques and provides a user-friendly interface for real-time predictions using Gradio.

**File:**
gradio_sms_text_classification.ipynb

**Challenges and Solutions:**
* Error when calling the function, found it could be that the "message" column has NaN values, so I handled the NaN value before we pass the data to TfidfVectorizer by using a custom preprocessor by converting the NaN values to an empty string, modifying the 'sms_classification' function.
* The X_test and y_test are not used in the current implementation. I modified the sms_classification function to include model evaluation using X_test and y_test.