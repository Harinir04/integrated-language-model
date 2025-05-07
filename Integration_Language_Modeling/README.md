# Integrated Language Modeling for Improved Accuracy in Transcription Services

# Overview
Project: OV Transcriber Description: This project is to use the standard messaging functionality in ov phone to improve transcription by using speech recognition and language models. In this project, we aim to transcribe audio to text, refine the transcription with the help of language models and store the original and the corrected transcriptions in a structured manner. This work is intended to improve the performance of dictation in speech-to-text systems by using a novel automatic text correction platform based on spoken and recognized text. The system would capture the audio with a microphone, transcribe that audio with the Google Speech API, and then resolve any transcription errors in the text using TextBlob. A comparison, finally, indicated that the Both the original and

# Technologies Used
1. SpeechRecognition: For recognizing and transcribing speech from the microphone.
2. TextBlob: For correcting the transcription errors by automatically correcting the text.
3. Datetime: To generate timestamps for saving the transcripts with unique filenames.
4. OS: For managing files and directories on the system.
5. PyAudio: Required for microphone input in the speech_recognition library.

# Requirements
1. Python 3.x
2. Libraries:
    -speechrecognition
    -textblob
    -pyaudio

# Installation
1. Install Python 3.x (if not already installed) from python.org.
2. Install the required libraries using pip:
    pip install SpeechRecognition textblob pyaudio
3. Download the necessary corpora for TextBlob:
    python -m textblob.download_corpora

# Usage
1. Clone the repository or save the script project3_transcript_language_model.py to your local machine.
2. Open your terminal or command prompt and navigate to the directory where the script is saved.
3. Run the script:
    python project3_transcript_language_model.py
4. The program will begin, and you will be prompted to speak. After a brief moment, the system will transcribe your speech.
5. The program will show both the original transcription and the corrected transcription.
6. Both transcriptions will be saved to a file in the corrected_transcripts/ directory with a timestamped filename.

# output
-Console Output
   Adjusting for background noise...
Start speaking...
Original Transcript: I am speking some tex
Corrected Transcript: I am speaking some text
✅ Transcript saved to corrected_transcripts/transcript_20230507_123456.txt

-Output Files
Original: I am speking some tex
Corrected: I am speaking some text

# Conclusion
The output of this project includes both the raw transcription and the corrected version. The raw transcription may contain errors due to background noise or mispronunciations. The corrected transcript, generated using TextBlob, shows the improved version, which corrects any spelling or grammatical mistakes. This integration of language modeling significantly enhances the accuracy of transcription services, especially in noisy environments.