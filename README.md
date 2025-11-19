# 🚀 SATHYA – Voice-Driven AI Assistant  
### A Python + Selenium + EEL Powered Desktop AI Assistant

<p align="center">
  <img width="700" src="https://dummyimage.com/1000x300/000/fff&text=SATHYA+-+AI+Assistant">
</p>

<p align="center">
  <b>Real-time Speech → AI Chat → UI Output</b><br>
  Built using Python, Selenium, STT automation & EEL for a smooth desktop interface.
</p>

---

### 📌 Project Overview – SATHYA Voice-Driven AI Assistant

SATHYA is a voice-driven AI assistant that I developed by integrating Python, Selenium automation, and an EEL-based desktop interface. The system processes voice commands end-to-end—starting with real-time speech recognition using a browser-based Speech-to-Text engine automated through Selenium. The converted text is saved to an input file, which is continuously monitored by a Logic Brain module. This module identifies valid commands, formats them, and sends them to an AI chat engine.

The AI engine is also automated using Selenium, where the assistant opens Pi AI, submits the query, extracts the response, and writes it to a response file. The desktop UI, built using HTML/CSS/JavaScript and rendered through EEL, refreshes every second and displays the AI’s answer in real time. All components—STT listener, logic processor, chat automation, and UI—run concurrently using Python multithreading, ensuring smooth and uninterrupted interaction.

This project demonstrates my ability to combine automation, Python scripting, multithreading, frontend integration, and real-time AI processing. It also highlights strong modular design, problem-solving skills, and end-to-end system architecture understanding.



### This project demonstrates:
✔ Real-time Speech-to-Text automation  
✔ Browser-based AI chat automation  
✔ Multi-threaded processing  
✔ Lightweight desktop UI  
✔ End-to-end integration between **Python, JavaScript, Selenium & AI**

---


## 🧠 How It Works

### **1️⃣ Speech-to-Text (STT.py)**
- Uses Selenium to automate a hosted STT web app  
- Writes converted text to:  
web/input.txt


### **2️⃣ Logic Brain (logic_brain.py)**
- Monitors `input.txt` for new STT output  
- Detects commands beginning with **"Sathya"**  
- Sends message to the chat engine  

### **3️⃣ Chat Engine (main.py)**
- Automates Pi AI using Selenium  
- Extracts AI response  
- Writes it to:  
web/response.txt


### **4️⃣ UI Layer (Sathya.py)**
- Renders `index.html` using EEL  
- Updates UI every second  
- Runs UI + brain + STT simultaneously using **threads**

---

## 🛡️ Badges
<p align="left">
  <img src="https://img.shields.io/badge/Status-Active-success?style=for-the-badge">
  <img src="https://img.shields.io/badge/Python-3.10+-blue?style=for-the-badge">
  <img src="https://img.shields.io/badge/Selenium-Automation-orange?style=for-the-badge">
  <img src="https://img.shields.io/badge/EEL-Frontend%20Bridge-green?style=for-the-badge">
  <img src="https://img.shields.io/badge/License-MIT-lightgrey?style=for-the-badge">
</p>

---

## 🗂 Project Structure
📦 SATHYA

├── logic_brain.py     # Brain logic (message monitor + dispatcher)

├── main.py            # Selenium AI chat automation

├── STT.py             # Real-time Speech-to-Text engine

├── Sathya.py          # EEL UI + threading orchestrator

├── web/

│ ├── input.txt        # Live STT output

│ ├── response.txt     # AI’s reply

│ ├── index.html       # UI interface

└── README.md


---

## 🧰 Technologies Used

### 🔹 **Programming & Frameworks**
- Python  
- Selenium WebDriver  
- EEL (Python ↔ JS bridge)  
- WebDriver Manager  

### 🔹 **Concepts**
- Multithreading  
- Browser automation  
- Explicit waits  
- Real-time STT  
- AI integration  
- File-based communication  

---

## 💡 Skill Set Demonstrated

### ✔ Python (Intermediate → Advanced)
- Modular scripting  
- Threading  
- Error handling  
- File operations  

### ✔ Automation (Selenium)
- Dynamic XPath  
- Headless browsers  
- Complex interactions  
- Authentication handlers  

### ✔ Frontend Integration (EEL)
- HTML/CSS/JavaScript UI  
- Live data updates  

### ✔ AI Integration
- Automated message sending  
- Response extraction  

### ✔ Software Architecture
- Multi-thread orchestration  
- Clean module separation  
- Real-time communication  

---

## ⚙️ Installation

### **1️⃣ Clone the Repository**
```bash
git clone https://github.com/your-username/SATHYA.git
cd SATHYA
```

### **2️⃣ Install Dependencies**
```bash
pip install selenium eel webdriver-manager
```
### **▶️ Running the Application**
``` bash
python Sathya.py
```
### Running this will:

Start the Speech-to-Text listener

Launch the AI processing engine

Open the desktop UI

Begin voice → AI → UI real-time streaming
