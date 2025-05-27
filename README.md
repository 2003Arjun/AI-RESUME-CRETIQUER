
# 📄 AI Resume Critiquer

The **AI Resume Critiquer** is a web application built with **Streamlit** that allows users to upload their resume (in PDF or TXT format) and receive intelligent, structured feedback to improve its effectiveness. The analysis is powered by OpenAI's GPT model.

---

## 🚀 Features

- 📄 Upload resumes in **PDF** or **TXT** format.
- 🧠 Get constructive and actionable **AI-generated feedback**.
- 🎯 Option to input the **target job role** for personalized suggestions.
- ⚡ Quick and interactive web interface using **Streamlit**.

---

## 🛠️ Tech Stack and Libraries Used

| Component         | Description                                             |
|------------------|---------------------------------------------------------|
| `Streamlit`      | For building the web interface.                         |
| `OpenAI`         | For analyzing and generating resume feedback.           |
| `PyPDF2`         | For extracting text from PDF resumes.                   |
| `dotenv`         | To securely manage the OpenAI API key via `.env`.       |
| `os`, `io`       | For file and environment handling.                      |

---

## 📂 Project Structure

```bash
.
├── app.py                 # Main Streamlit app file
├── .env                  # Stores your OpenAI API key (not committed)
├── requirements.txt      # Required libraries
└── README.md             # Project documentation
````

---

## 🔧 Installation & Setup

### ✅ 1. Clone the Repository

```bash
git clone https://github.com/your-username/ai-resume-critiquer.git
cd ai-resume-critiquer
```

### ✅ 2. Create and Activate a Virtual Environment (optional but recommended)

```bash
# Windows
python -m venv venv
venv\Scripts\activate

# macOS/Linux
python3 -m venv venv
source venv/bin/activate
```

### ✅ 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### ✅ 4. Set Up OpenAI API Key

Create a `.env` file in the root folder and add your OpenAI key:

```
OPENAI_API_KEY=your_openai_api_key_here
```

---

## ▶️ Running the App

Once everything is set up, run the app using:

```bash
streamlit run app.py
```

This will launch the web app in your default browser.

---

## 📷 Screenshots

![App Screenshot](https://via.placeholder.com/800x400.png?text=Upload+Resume+Screenshot)
*Upload screen*

![Feedback Screenshot](https://via.placeholder.com/800x400.png?text=AI+Feedback+Screenshot)
*AI-generated feedback*

---

## 🧠 How it Works

1. The user uploads a resume (PDF or TXT).
2. The resume content is extracted using `PyPDF2` or decoded directly if it's a `.txt` file.
3. An analysis prompt is dynamically generated and sent to OpenAI GPT (via `gpt-4o`).
4. GPT responds with constructive feedback based on job role and resume content.
5. The response is displayed in the Streamlit interface.

---

## 🔮 Future Upgrades

Here are some ideas for future enhancements:

* ✅ **Job Description Upload:** Allow users to upload a JD for more tailored suggestions.
* 🌐 **Multilingual Support:** Accept resumes in other languages.
* 📊 **Score System:** Give a numerical score for each section (skills, layout, etc.).
* 🖼️ **PDF Annotator:** Provide direct annotations or highlights on PDF resumes.
* 🧩 **Cover Letter Generator:** Automatically suggest or generate cover letters.
* 📂 **Save Feedback:** Allow users to download or email their feedback.
* 🔐 **User Authentication:** Support for account-based access and resume history.

---

## ❓ Troubleshooting

* Ensure your `.env` file is present and correctly configured.
* Make sure you’re connected to the internet while using the app.
* Use only `.pdf` or `.txt` files for uploads.
* If errors persist, check logs in the terminal for more details.

---

## 📃 License

This project is licensed under the [MIT License](LICENSE).

---

## 🙌 Acknowledgements

* [OpenAI](https://openai.com/)
* [Streamlit](https://streamlit.io/)
* [PyPDF2](https://pypi.org/project/PyPDF2/)

---

## ✉️ Contact

For any questions or suggestions, reach out to:

**Your Name**
Email: [youremail@example.com](mailto:youremail@example.com)
GitHub: [@your-username](https://github.com/your-username)

---

````

---

## 🔁 Don't Forget

Create a `requirements.txt`:

```bash
pip freeze > requirements.txt
````

And your `.env` should **not be committed to GitHub** — add this to `.gitignore`:

```
.env
```


