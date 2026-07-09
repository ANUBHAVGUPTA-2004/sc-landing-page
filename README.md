# SnapClass — AI-Powered Smart Attendance System 🎓

SnapClass is an AI-powered classroom attendance system that automates attendance marking using **face recognition** and **voice verification**, eliminating proxy attendance and manual roll calls. With a single classroom photo, SnapClass can detect and mark attendance for an entire class in seconds.

---

## ✨ Features

- 🧠 **AI Face Recognition** — Detects and marks attendance for an entire class from a single classroom photo, using face recognition models to match students against enrolled faces.
- 🎙️ **Voice Verification** — Adds an extra layer of identity confirmation using voice biometrics to eliminate proxy attendance.
- 📷 **QR-Based Roster System** — Students can instantly enroll in a course by scanning a QR code, streamlining the onboarding process.
- 📊 **Real-Time Analytics Dashboard** — View attendance history, AI confidence scores, and trends at a glance.
- 📁 **CSV Export** — Export attendance records for record-keeping and reporting.
- ☁️ **Cloud Backend with Supabase** — Reliable, real-time backend for storing attendance data, student records, and course information.

---

## 🛠️ Tech Stack

**Backend & AI**
- Python
- Flask
- Face Recognition (`face_recognition` / Dlib)
- Resemblyzer (voice embeddings for speaker verification)
- Librosa (audio processing)

**Frontend / App**
- Streamlit

**Database & Backend-as-a-Service**
- Supabase
- PostgreSQL

---

## 🚀 How It Works

1. **Enroll Students** — Students enroll in a course by scanning a QR code linked to the class roster.
2. **Capture Attendance** — A teacher takes a single photo of the classroom.
3. **AI Face Detection** — The system detects all faces in the photo and matches them against enrolled student profiles.
4. **Voice Verification (optional layer)** — Voice samples are used to further confirm identity and prevent proxy attendance.
5. **Attendance Logged** — Matched students are automatically marked present, with confidence scores stored in Supabase.
6. **View & Export** — Teachers can view real-time analytics on the dashboard and export attendance as CSV.

---

## ⚙️ Setup & Installation

1. **Clone this repository**
   ```bash
   git clone https://github.com/ANUBHAVGUPTA-2004/Snapclass-AI---Attendance.git
   cd Snapclass-AI---Attendance
   ```

2. **Create a virtual environment**
   ```bash
   python -m venv venv
   source venv/bin/activate   # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Set up Supabase**
   - Create a project on [Supabase](https://supabase.com)
   - Add your Supabase URL and API key to your environment configuration file (e.g. `.env` or `config.py`)

5. **Run the app**
   ```bash
   streamlit run app.py
   ```

---

## 📂 Project Structure

```
Snapclass-AI---Attendance/
├── src/                # Core application logic (face recognition, voice verification, etc.)
├── app.py              # Main Streamlit application entry point
├── requirements.txt    # Python dependencies
└── .gitignore
```

---

## 🌐 Live Links

- **Landing Page:** [sc-landing-page-livid-eight.vercel.app](https://sc-landing-page-livid-eight.vercel.app)
- **GitHub Repository:** [SnapClass AI — Attendance](https://github.com/ANUBHAVGUPTA-2004/Snapclass-AI---Attendance)

> ⚠️ Note: If hosted on Streamlit Community Cloud, the live demo may go to sleep after a period of inactivity. Simply click **"Yes, get this app back up!"** to wake it — it takes about 1–2 minutes to restart.

---

## 🔮 Future Improvements

- Mobile app support for on-the-go attendance capture
- Multi-classroom / multi-section support with admin roles
- Automated email/SMS alerts for low attendance
- Improved low-light face detection accuracy

---

## 👤 Author

**Anubhav Gupta**
[GitHub](https://github.com/ANUBHAVGUPTA-2004)

---

## 📄 License

This project is currently unlicensed. Feel free to reach out for usage permissions.
