# **Voice-to-Text & Recorder**

A powerful, browser-based dictation application that provides real-time voice-to-text transcription, audio recording, and local folder management. This single-page application is built with vanilla JavaScript, leveraging modern browser APIs to deliver a seamless and efficient user experience without requiring a backend.

## **Features**

* **Real-Time Transcription:** Uses the browser's Web Speech API for fast and accurate voice-to-text conversion.  
* **Multilingual Support:** Choose from a wide range of languages for transcription.  
* **Audio Recording:** Simultaneously records your voice and saves the original high-quality .webm audio.  
* **Pause & Resume:** Easily pause and resume your recording sessions without losing your progress.  
* **On-Demand MP3 Export:** Convert your .webm recordings to the universally compatible .mp3 format with a single click, powered by a client-side lamejs encoder.  
* **Folder Management:** Organize your recordings into folders. Create new folders and filter your recordings for better organization.  
* **Persistent Local Storage:** All recordings and folders are saved locally and securely in your browser using **IndexedDB**, ensuring your data persists across sessions and can handle large files without quota errors.  
* **Rich Playback Interface:**  
  * Play back any recording directly from the list.  
  * View detailed stats for each recording, including title, word count, audio duration, file size, and a relative timestamp (e.g., "5 minutes ago").  
  * Expand recordings to view the full transcription.  
* **Modern & Responsive UI:** Clean, intuitive, and mobile-friendly interface built with Tailwind CSS.

## **Tech Stack**

* **Frontend:** HTML5, CSS3, Vanilla JavaScript (ES6+)  
* **Styling:** Tailwind CSS  
* **Browser APIs:**  
  * **Web Speech API (SpeechRecognition)**: For voice-to-text transcription.  
  * **MediaRecorder API**: For audio capture.  
  * **IndexedDB**: For robust, client-side storage of large files and data.  
* **Libraries:**  
  * **lamejs**: A JavaScript MP3 encoder for client-side audio conversion.

## **How to Use**

1. **Open the Application:** Simply open the index.html file in a supported web browser.  
2. **Allow Permissions:** The browser will ask for microphone permission. Please allow it to enable recording.  
3. **Select a Folder:** Choose a folder from the dropdown or create a new one using the "+" button. Your recording will be saved to the selected folder.  
4. **Choose Your Language:** Select your desired language from the dropdown menu on the left.  
5. **Start Recording:** Click the **Start** button and begin speaking. Your words will appear in the text area in real-time.  
6. **Control Your Recording:**  
   * Click **Pause** to temporarily stop the recording.  
   * Click **Resume** to continue.  
   * Click **Stop** to finalize the recording.  
7. **Manage Recordings:**  
   * Click on any recording in the list to expand it and view the full transcription.  
   * Use the icons to **Play**, **Copy Text**, **Download WebM**, **Download as MP3**, or **Delete** the recording.

## **Browser Compatibility**

This application relies on modern browser APIs. For the best experience, please use:

* **Google Chrome** (Desktop & Android)  
* **Microsoft Edge** (Chromium version)

**Not Supported:**

* **Safari (macOS & iOS):** Apple has not implemented the Web Speech API in WebKit, so transcription will not work.  
* **Any browser on iOS (iPhone/iPad):** Due to Apple's restrictions, no browser on iOS supports the Web Speech API.  
* **Firefox:** While it has some support, it may not be as stable as on Chromium-based browsers.
