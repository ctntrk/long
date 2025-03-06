# Long YouTube Video Summarizer

This script automates the process of downloading an audio file from a YouTube video, transcribing it into text, and summarizing the content. It also measures the time taken for each step, providing performance insights, and displays the results, including the transcript and summary along with character and word counts.

# Purpose:
- **Download** audio from a YouTube video.
- **Transcribe** the audio into text using OpenAI’s Whisper model.
- **Summarize** the transcribed text using the BART model from Hugging Face.
- **Display statistics**: Character and word counts for both the transcript and summary.
- **Measure performance**: Time taken for each process (downloading, transcribing, summarizing).

# Features:
- **Audio Download**: Uses `yt-dlp` to download the best quality audio from YouTube.
- **Transcription**: Leverages OpenAI's Whisper model to convert audio to text.
- **Summarization**: Uses Hugging Face's BART model to summarize the transcribed text into a concise form.
- **Performance Tracking**: Tracks the time for each step and displays it, including download time, transcription time, and summarization time.
- **Statistics**: Outputs the word and character counts for both the transcript and the summary.

# Libraries Used:
- `yt-dlp`: For downloading YouTube videos and audio.
- `openai-whisper`: For transcribing audio files into text.
- `transformers`: For text summarization.
- `torch`: Required for running AI models.

# Comparison to Similar Code:
- The current code (Code A) adds time tracking and batch processing capabilities compared to an earlier version (Code B), making it more structured and automated.
- Code A processes multiple YouTube URLs dynamically using a loop, while Code B is more manual and focused on processing single URLs sequentially.
- Code A includes detailed performance insights (time tracking), while Code B does not focus on performance measurement.

# Summary:
This script is designed to automate the process of downloading YouTube audio, transcribing it, and summarizing the content, with detailed performance tracking. It is useful for efficiently processing and analyzing multiple videos in a batch while keeping track of processing times for each step.
