# 🎥 AI Video Assistant

An AI-powered **Multimodal Video Assistant** that understands video and audio content using **OpenAI GPT-4o**, **Whisper**, **Text-to-Speech (TTS)**, and **Shiny for Python**.

The application allows users to upload a video, automatically extracts audio and video frames, transcribes speech using Whisper, analyzes both visual and spoken content with GPT-4o (or LLaVA), and returns a spoken AI response. It also includes a model comparison interface to evaluate GPT-4o, GPT-4 Vision, and LLaVA-7B side by side. :contentReference[oaicite:0]{index=0} :contentReference[oaicite:1]{index=1}

---

## 🚀 Features

- Upload and analyze video files
- Automatic audio extraction from videos
- Video frame extraction
- Speech-to-text using OpenAI Whisper
- Multimodal understanding with GPT-4o
- AI-generated spoken responses
- Text-to-Speech (TTS) output
- Interactive Shiny web interface
- Compare GPT-4o, GPT-4 Vision, and LLaVA-7B
- Local LLaVA support using Ollama

---

## 📊 Application Workflow

The application performs:

- Video Upload
- Audio Extraction
- Frame Extraction
- Speech Transcription
- AI Video Understanding
- Spoken Response Generation
- Model Comparison Dashboard

---

## 🏗️ Project Architecture

```
                    User
                      │
                      ▼
                Upload Video
                      │
                      ▼
             Video Processing
                      │
          ┌───────────┴───────────┐
          ▼                       ▼
   Audio Extraction        Frame Extraction
          │                       │
          ▼                       ▼
   OpenAI Whisper          Video Frames
          │                       │
          └───────────┬───────────┘
                      ▼
              User Prompt Created
                      │
                      ▼
      GPT-4o / GPT-4 Vision / LLaVA
                      │
                      ▼
          AI Response Generation
                      │
                      ▼
        OpenAI Text-to-Speech (TTS)
                      │
                      ▼
            Audio Response (MP3)
                      │
                      ▼
             Shiny Web Interface
```

---

# 📁 Project Structure

```
AI-Video-Assistant/

│── app.py
│── app_bakeoff.py
│── query.py
│── query_bakeoff.py
│── video-to-speech.ipynb
│── system_prompt.txt
│── input.mov
│── requirements.txt
│── README.md
```

---

# 🛠 Technologies Used

### Programming

- Python

### AI Models

- OpenAI GPT-4o
- GPT-4 Vision
- Whisper
- OpenAI Text-to-Speech
- LLaVA-7B (Ollama)

### Framework

- Shiny for Python

### Video Processing

- FFmpeg

### Libraries

- OpenAI SDK
- Pandas
- Matplotlib
- Python-dotenv
- Ollama

---

# ⚙️ Installation

Clone the repository

```bash
git clone https://github.com/yourusername/ai-video-assistant.git

cd ai-video-assistant
```

Install dependencies

```bash
pip install -r requirements.txt
```

Install FFmpeg

Windows

```bash
choco install ffmpeg
```

macOS

```bash
brew install ffmpeg
```

Install Ollama (Optional)

```bash
ollama pull llava:7b
```

---

# 🔑 Environment Variables

Create a `.env` file and configure:

```
OPENAI_API_KEY=your_openai_api_key
```

---

# ▶️ Running the Project

Run the notebook

```bash
jupyter notebook video-to-speech.ipynb
```

Run the interactive Shiny application

```bash
shiny run app.py --port 0 --launch-browser
```

Run the model comparison application

```bash
shiny run app_bakeoff.py --port 0 --launch-browser
```

---

# 📌 Workflow

1. Upload a video.
2. Extract audio and video frames from the uploaded file.
3. Convert speech into text using OpenAI Whisper.
4. Combine the transcription with extracted video frames.
5. Send multimodal input to GPT-4o, GPT-4 Vision, or LLaVA.
6. Generate an AI response based on both visual and spoken content.
7. Convert the response into speech using OpenAI Text-to-Speech.
8. Play the generated audio response in the Shiny interface.

---

# 📈 Application Features

The application includes:

- Video upload interface
- Speech transcription
- AI-powered video understanding
- Audio response generation
- Progress indicators
- Interactive model comparison
- Performance benchmarking

---

# 📚 Learning Outcomes

This project helped in learning:

- Multimodal AI
- GPT-4o Integration
- OpenAI Whisper
- OpenAI Text-to-Speech
- Video Processing with FFmpeg
- Prompt Engineering
- Shiny for Python
- LLaVA Integration
- Ollama
- AI Model Comparison
- Asynchronous Programming

---

# 🔮 Future Enhancements

- Live webcam support
- Real-time video analysis
- Emotion detection
- Object detection
- OCR from videos
- Multi-language speech recognition
- Subtitle generation
- Video summarization
- Video question answering
- Cloud deployment

---

# 📄 Disclaimer

This project is developed for educational and portfolio purposes. It demonstrates multimodal AI by combining video processing, speech recognition, large language models, and text-to-speech technologies to create an intelligent video assistant capable of understanding and responding to uploaded videos.
