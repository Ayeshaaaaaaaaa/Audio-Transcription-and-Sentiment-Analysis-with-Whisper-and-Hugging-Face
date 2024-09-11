# Audio-Transcription-and-Sentiment-Analysis-with-Whisper-and-Hugging-Face
This project combines audio transcription using OpenAI's Whisper model and sentiment analysis using the Hugging Face distilbert-base-uncased-finetuned-sst-2-english model. It first transcribes audio files into text and then processes the transcription in chunks to analyze the sentiment of each segment.
# Features
Audio Transcription: Uses OpenAI Whisper's medium model to transcribe audio files into text.
Sentiment Analysis: Sentiment analysis on the transcribed text using Hugging Face Inference API with DistilBERT.
Text Chunking: Splits large transcriptions into manageable chunks within the model's token limit (512 tokens).
Simple Tokenization: Basic space-based tokenization for chunking before analysis.
# Project Structure
transcription.py: Script for transcribing audio files using Whisper.
sentiment_analysis.py: Contains logic for performing sentiment analysis on the transcribed text.
requirements.txt: Lists the required Python libraries (e.g., whisper, requests).
# How to Run
# Transcription:

Provide an audio file, and the Whisper model will transcribe it into text.
![image](https://github.com/user-attachments/assets/badedeec-8594-4a24-a73e-203a078a2384)
# Sentiment Analysis:

The transcribed text is chunked, and each chunk is analyzed for sentiment using the Hugging Face API.
![image](https://github.com/user-attachments/assets/ed935043-f0c1-466b-9cb8-7f0aff7ee853)
# API Integration
Hugging Face model: distilbert-base-uncased-finetuned-sst-2-english
API URL: https://api-inference.huggingface.co/models/distilbert-base-uncased-finetuned-sst-2-english
# Requirements
whisper
requests
# Example Workflow
Transcribe the audio using Whisper.
Perform sentiment analysis on the transcribed text.
Print sentiment results for each chunk of the transcription.

