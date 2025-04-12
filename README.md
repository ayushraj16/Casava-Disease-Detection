
# 🌿 Cassava Leaf Disease Detection using Google Gemini + Gradio

This is a web-based AI tool that helps **detect diseases in cassava leaves** by analyzing uploaded images using Google's **Gemini 1.5 Flash** model. The application provides detailed diagnosis, symptoms, causes, treatment, and prevention suggestions in a simple Gradio interface.

---

## 🚀 Features

- Upload multiple cassava leaf images.
- Analyze each image with AI to detect diseases (or confirm healthy leaves).
- Get detailed results including:
  - Disease name
  - Symptoms
  - Causes
  - Treatment
  - Prevention tips
- Simple web interface using [Gradio](https://www.gradio.app/).

---

## 📸 How It Works

1. User uploads one or more cassava leaf images.
2. Each image is passed along with a descriptive prompt to the **Gemini 1.5 Flash model** via Google’s Generative AI SDK.
3. AI analyzes the image and returns a structured, human-readable analysis.
4. Results are displayed in a table for easy comparison.

---

## 🧠 Tech Stack

- **Google Generative AI SDK** – Uses Gemini 1.5 Flash for image analysis.
- **Gradio** – For building a user-friendly front-end.
- **Pandas** – To structure and display output as a DataFrame.
- **Python** – Core language for all operations.

---

## 📁 File Structure

```
cassava-disease-detector/
│
├── app.py                   # Main Gradio application
├── README.md                # This file
├── requirements.txt         # Required packages
└── ...
```

---

## 🛠️ Setup Instructions

1. **Clone the repository:**
```bash
git clone https://github.com/your-username/cassava-disease-detector.git
cd cassava-disease-detector
```

2. **Install dependencies:**
```bash
pip install -r requirements.txt
```

3. **Set your API key:**
Replace your Gemini API key inside `app.py`:
```python
client = genai.Client(api_key="YOUR_API_KEY_HERE")
```

4. **Run the app:**
```bash
python app.py
```

5. Open the Gradio interface in your browser!

---

## 🔐 Note on API Key

This app uses the **Google Generative AI API** — you'll need access to [Google AI Studio](https://aistudio.google.com/) and a valid API key.

---

## 🧪 Example Use Case

Upload a few cassava leaf images (JPEG or PNG). The app will analyze them like:

| Image      | Analysis |
|------------|----------|
| Image 1    | Disease: Cassava Mosaic Virus... |
| Image 2    | The leaf appears healthy...      |

---

## 🤖 Prompt Used Behind the Scenes

```text
Analyze this image of a cassava leaf and identify any potential diseases.
Provide a comprehensive analysis with the following:
1. Disease Name (if present)
2. Symptoms visible in the image
3. Potential causes
4. Recommended treatments
5. Prevention measures
```

---

## 📸 Screenshots

*(Add screenshots or demo gifs here if you have them!)*
![image](https://github.com/user-attachments/assets/25809b79-c3d0-405d-a895-fffa3a394b1c)

## 🤝 Contributing

Pull requests are welcome! Feel free to open issues or suggest features.

---

## 📜 License

This project is open-source under the [MIT License](LICENSE).
