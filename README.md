# VidChat-Chat-with-YouTube

![1 (1)](https://github.com/user-attachments/assets/998ca82d-98e5-49ad-b9cc-f7bd057ccf0e)


VidChat: Chat with YouTube!
This project allows users to interact with YouTube videos through questions, either by entering a video URL or searching for videos based on keywords. The app transcribes video content and provides answers to user queries using the video transcript.

Key Components:

- app.py
Central app file using Streamlit, featuring two modes:

- URL-based interaction: Users enter a YouTube URL, and the app generates answers based on the video transcript.
- Search-based interaction: Users search for videos by keywords and ask questions about the selected video.

- youtubevideo.py
Defines the YoutubeVideo class to manage video properties like ID, title, and URL.

- raghelper.py
Handles Retrieval-Augmented Generation (RAG) using video transcripts and AI models (Google Gemini, OpenAI). Retrieves relevant transcript parts to generate responses.

- videohelper.py
Provides video transcription (using Whisper) and search functions (using Scrapetube).

- How It Works:

Input (URL or Search): Users provide a video URL or search for one.

Transcription: The video is transcribed into text.

Query: Users ask questions, and the system retrieves transcript parts to answer.

Response: AI generates answers using RAG.

Technologies:
- Streamlit, Langchain, Whisper, Google Gemini, Scrapetube, FAISS
