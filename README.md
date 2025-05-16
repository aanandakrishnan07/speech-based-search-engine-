# speech-based-search-engine-


---

### 🔧 **Functionality Overview**

1. **Uses Microphone Input**:

   * Prompts the user to speak using their microphone.

2. **Speech Recognition**:

   * Uses Google's speech recognition API via the `speech_recognition` library.

3. **Performs a Google Search**:

   * Opens a browser with Google search results for the recognized speech.

4. **Text-to-Speech Feedback**:

   * Uses `pyttsx3` to speak prompts and feedback to the user.

---

### 🧩 **Key Components**

* **Libraries Used**:

  ```python
  import speech_recognition as sr
  import pyttsx3
  import webbrowser
  ```

* **Text-to-Speech Function**:

  ```python
  def speak(text):
      engine.say(text)
      engine.runAndWait()
  ```

* **Listening and Recognizing Speech**:

  ```python
  def take_command():
      ...
      audio = r.listen(source)
      query = r.recognize_google(audio)
      return query
  ```

* **Searching the Web**:

  ```python
  def search_web(query):
      url = f"https://www.google.com/search?q={query}"
      webbrowser.open(url)
  ```

* **Main Execution**:

  ```python
  if __name__ == "__main__":
      query = take_command()
      search_web(query)
  ```

---

### ▶️ **How to Run**

1. Install required libraries:

   ```bash
   pip install SpeechRecognition pyttsx3 pyaudio
   ```

2. Run the script:

   ```bash
   python "speech based search engine (2).py"
   ```

3. Speak when prompted. It will recognize your speech and perform a Google search.

---

