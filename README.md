Interview Simulation Using LLM

This Interview Simulation App is built with Streamlit, Google SpeechtoText, and LangChain to deliver a conversational AIdriven experience. It enables users to record answers to interview questions, transcribe their responses using Google’s SpeechtoText API, and create lipsynced videos of an avatar presenting the next question. LangChain and Groq’s AI model power the avatar and conversation flow.  


Functionality:

1. Start Interview:
    The user uploads a resume.  
    AI generates interview questions tailored to the resume and selected interview type.  
    The first question is displayed alongside a video of the avatar asking the question.  

2. Record Answers:
    The user clicks a button to record their answer.  
    The recorded audio is transcribed to text using Google SpeechtoText.  

3. Process Answer and Generate Video:
    The transcribed response is processed by LangChain to generate the next question.  
    A lipsynced video of the avatar presenting the new question is created.  

4. Repeat Process:
    The cycle continues for a predefined number of questions (default: 5).  

5. Evaluation:
    After answering all questions, the app evaluates the interview and provides feedback on the user's performance.  

API Integrations:

1. Google SpeechtoText:
    Used to transcribe the user's voice into text.  
    Requires the user to provide their own API credentials.  

2. Groq API:
    Powers conversational AI to generate interview questions based on the uploaded resume.  
    Called to fetch AI responses throughout the interview process.  
