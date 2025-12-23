# AI Handwritten Math Solver – Frontend

This repository contains the **frontend** of the AI Handwritten Math Solver project.  
The application uses the device camera to scan handwritten or printed mathematical problems, performs OCR directly in the browser, and sends the extracted expression to a cloud-based AI backend for solving.

The frontend is packaged as an **Android APK** using Capacitor.

---

## ✨ Features

- 📷 Rear camera capture for scanning math problems  
- 🔍 OCR using **Tesseract.js** (runs fully on-device)  
- 🧠 AI-powered step-by-step math solving via backend API  
- 📐 Proper math rendering using **LaTeX (KaTeX)**  
- 📱 Packaged as an Android application (APK)  
- 🌐 Works over HTTPS with a deployed cloud backend  

---

## 🏗️ Architecture Overview


- The frontend handles **image capture, OCR, and UI**
- The backend handles **AI reasoning and math solving**
- Communication is done via a REST API

---

## 🧰 Tech Stack

- **HTML, CSS, JavaScript**
- **Tailwind CSS** – UI styling
- **Tesseract.js** – Optical Character Recognition
- **KaTeX** – Mathematical expression rendering
- **Capacitor** – Android APK packaging

---

## 🚀 How It Works

1. The user captures an image of a math problem using the phone camera  
2. The image is processed and converted to text using OCR  
3. Extracted math text is sent to the backend API  
4. The backend returns a step-by-step solution  
5. The solution is rendered in a readable mathematical format   

---

## 🔧 Local Development

## Prerequisites
- Node.js
- npm
- Android Studio (for APK build)
- Capacitor CLI

 Install dependencies
``bash##

___
### npm install



Sync frontend with Android project
npx cap sync

Build APK (debug)
cd android
./gradlew assembleDebug


APK output:

android/app/build/outputs/apk/debug/app-debug.apk

###🌐 Backend Integration

The frontend communicates with a deployed backend API.

Example endpoint used in the code:

https://ai-math-backend-xscf.onrender.com/solve


Request format:

{
  "image": "2x + 3 = 7"  
}

ai-math-frontend/
├── index.html
├── package.json
├── capacitor.config.json
├── android/        (generated, ignored in git)
├── www/            (generated, ignored in git)


### 📜 License

This project is intended for educational and academic use.

---

### ✅ WHY THIS README IS GOOD

- Clear and structured  
- Explains **what**, **how**, and **why**  
- No fake claims  
- Easy for examiners to understand  
- Looks like a real GitHub project, not a tutorial dump  

If you want next:
- **Backend README**
- **Project abstract**
- **Architecture diagram**
- **Viva questions & answers**
- **Final submission checklist**


