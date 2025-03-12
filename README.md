
<h1 align='center' style=color:#fe5e21;><strong>Automatic Bangla Transcription</strong></h1>

A system that takes bangla audio files as inputs and returns a csv/excel file containing transcriptions of all of those audio files. This is an ongoing project and I'm responsible for the AI and Automatic Transcription aspects of this project.

<br/>

<h2 style=color:#fe5e21;>System  Development</h2>

Since there are no free Bangla Transcription websites that take in audio and return their transcriptions, I decided to build a system and deploy it on the internet where a user can upload Bangla speech audios and the system will return all the transcriptions in a single file.

So far, I developed a prototype version of the system for it to be integrated later in a website will full-fledged frontend and backend. The system will take any formatted audio files and runs operations and relevant processing of those audio files within the system to ease the user experience and after being done with the processings, will return transcriptions of those different audio files in a single CSV/excel file.

I'm using an advanced model checkpoint to automatically transcribe the audios but one of the shortcomings of the model is it cannot process long audio files so I'm using another model through an API call that will split the audio data based on the vocal activity and filter out the silence parts to reduce the overall duration of the audio file and then will send these chunks to the transcription model work on.

**Automatic Bangla Transcription**

The model can transcribe standard Bangla speech with great accuracy but struggles to transcribe non-Bengali words or regional dialects in the speech.

**Prototype model transcription**

I have done a prototype test of the system with different audio files of different audio formats and different lengths and the screenshot below shows the full automated transcription time and relevant information regarding the transcription process of those audio.

![automated transcripton screenshot](https://raw.githubusercontent.com/RezuwanHassan262/Automatic-Bangla-Transcription/main/images/Output_Screenshot.PNG) 


<h3 style=color:#fe5e21;>Note</h3>

Model outputs alone cannot be fully trusted for such tasks; human validation is essential before real-world application.



