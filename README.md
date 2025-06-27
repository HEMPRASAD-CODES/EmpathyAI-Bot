# EmpathyAI-Bot

Overview
This project implements an advanced emotion-aware chatbot that combines quantum machine learning and deep learning to detect, classify, and respond to human emotions in text conversations. The chatbot aims to deliver empathetic, context-aware, and emotionally intelligent interactions, making it suitable for mental health support, education, and human-computer interaction scenarios.

Key Features
Quantum-Enhanced Emotion Classification:
Utilizes a hybrid quantum-classical neural network (built with PennyLane and PyTorch) to classify user input into six emotion categories: neutral, sadness, anxiety, anger, hopelessness, and loneliness.

Classical NLP Integration:
Leverages transformer-based language models (e.g., Llama2) for generating contextually appropriate, supportive responses.

Synthetic and Real-World Data:
Trains the emotion classifier using a mix of synthetic examples and real-world datasets (GoEmotions, Twitter emotion datasets), ensuring robust emotion detection across diverse text inputs.

Contextual Memory:
Maintains conversation and emotion history for each user, enabling the chatbot to reference previous topics, track emotional trends, and personalize responses over time.

Safety and Crisis Detection:
Includes keyword-based crisis detection to provide immediate support resources if users mention self-harm or crisis-related language.

Interactive and Modular:
The chatbot can be run interactively, supports special commands for debugging and memory management, and is designed for easy extension and deployment.

How It Works
Emotion Detection:
User messages are encoded using a sentence transformer and passed to the quantum-classical emotion classifier. The predicted emotion and confidence score guide the chatbot’s response style.

Response Generation:
The chatbot generates responses using a transformer-based language model, conditioning its output on detected emotions, conversation history, and user-specific context.

Memory and Personalization:
The system tracks user emotions, conversation topics, and trends, allowing it to adapt its responses and provide more personalized, empathetic support.

Safety Monitoring:
If crisis keywords are detected, the chatbot immediately shares mental health resources and encourages the user to seek professional help.

Technologies Used
Quantum Machine Learning: PennyLane, PyTorch

Natural Language Processing: Hugging Face Transformers, Sentence Transformers

Classical ML: scikit-learn, XGBoost (for baseline comparisons)

Utilities: NumPy, pandas, Streamlit (for UI), LangChain (for memory/context)

Deployment: Python 3, GPU acceleration (optional)

Use Cases
Mental health and emotional support chatbots

Emotion-aware conversational agents for education and customer service

Research in quantum machine learning for NLP

