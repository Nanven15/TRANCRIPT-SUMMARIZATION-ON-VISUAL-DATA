# TRANCRIPT-SUMMARIZATION-ON-VISUAL-DATA
This project leverages NLP to summarize YouTube transcripts into short, medium, or large lengths, with added translation, text-to-speech, and keyword search features for enhanced accessibility and information retrieval.


### **Overview of the Project:**
This AI project utilizes **Natural Language Processing (NLP)** techniques to summarize YouTube video transcripts. It allows users to input a YouTube video URL, fetch the transcript, and generate a summary. The summarization can be customized to different sizes (e.g., short, medium, or long). In addition, the project includes features like **translation** of the summarized transcript into other languages, **text-to-speech** (TTS) conversion, and a **keyword search** function to quickly find specific information in the summarized text.

### **Key Features and Workflow:**
1. **Transcript Fetching:**
   - The system uses the **YouTubeTranscriptApi** library to fetch transcripts from YouTube videos by parsing the video URL.
   
2. **Summarization:**
   - The summarization is done by loading the text into **spaCy**, a powerful NLP library.
   - It processes the transcript, tokenizes the text, and removes stopwords and punctuation.
   - Sentences are scored based on word frequencies, and the most significant ones are selected to form the summary.
   - Users can select the length of the summary (short, medium, long), and the system generates summaries accordingly.

3. **Translation:**
   - The project includes a **translation feature** that allows the summarized transcript to be translated into other languages (like Sinhala or Tamil) using the **Translator** library.
   
4. **Text-to-Speech:**
   - Once the summary is generated, it can be converted into speech using the **gTTS (Google Text-to-Speech)** library, enabling an auditory output of the summary.

5. **Keyword Search:**
   - A special feature allows users to **search for specific keywords** within the summarized data, providing more flexibility in finding particular points of interest.

6. **CPU & Memory Monitoring:**
   - The project monitors CPU and memory usage using the **psutil** library, likely to keep track of system performance while handling larger transcripts.

### **Tech Stack and Tools:**
- Python as the primary programming language.
- spaCy for NLP tasks like tokenization and text processing.
- YouTubeTranscriptApi to retrieve transcripts from YouTube.
- gTTS for text-to-speech conversion.
- Translator for language translation.
- Tkinter for building the graphical user interface (GUI).
- psutil for system performance monitoring.

 Additional Functionality:
- User Interface (UI): The project seems to use **Tkinter** for creating a simple graphical user interface, allowing users to input URLs, view results, and control summarization settings.

This project demonstrates practical applications of NLP, such as summarization, translation, and keyword search, while integrating different media formats like audio. It’s well-suited for users seeking quick and customizable summaries of YouTube content, offering a comprehensive solution with an intuitive interface.

