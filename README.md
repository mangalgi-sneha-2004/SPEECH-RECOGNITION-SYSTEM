# SPEECH-RECOGNITION-SYSTEM

COMPANY:CODTECH IT SOLUTIONS

NAME:MANGALGI SNEHA

INTERN-ID:CTO4WT53

DOMAIN:ARTIFICIAL INTELLIGENCE

DURATION:4 WEEKS

DESCRIPTION:

This Python script performs speech-to-text transcription using Facebook's Wav2Vec2 model from the Hugging Face Transformers library. It converts an audio file (e.g., MP3, WAV) into text while also visualizing the 

audio waveform and allowing playback (in Jupyter Notebook).


Key Steps & Features:

Initial Setup & Warnings Handling

The code suppresses unnecessary warnings (e.g., model weight mismatches, future deprecations) for cleaner output.

File Existence Check

Before processing, it verifies if the input audio file exists using Path(audio_path).exists().

Model Loading

Uses Wav2Vec2Processor (for audio preprocessing) and Wav2Vec2ForCTC (for speech recognition).

Automatically downloads the "facebook/wav2vec2-base-960h" model on first run.

GPU/CPU Detection

Checks for CUDA (GPU) support with torch.cuda.is_available() and loads the model onto the appropriate device.

Audio Loading

Uses librosa (default) to load audio at 16kHz sampling rate.

Falls back to pydub if librosa fails (useful for Windows compatibility).

Audio Visualization & Playback

Plots the waveform using matplotlib for visual inspection.

Embeds an interactive audio player in Jupyter Notebook via IPython.display.Audio.

Speech Recognition

Processes audio through the model using PyTorch’s autocast (for GPU efficiency).

Decodes the output into text with processor.batch_decode().

Error Handling

Catches and displays errors (e.g., file not found, audio loading issues).

OUTPUT:

![Image](https://github.com/user-attachments/assets/81658eeb-a31d-4466-831c-ec35ad25e787)


