# **SwarSetu**

## **Project Overview**

**SWar (SwarSetu)** is an intelligent real-time **Sign Language Recognition and Communication Platform** designed to bridge the communication gap between sign language users and verbal communication users. The system captures hand gestures through a webcam, detects the performed sign using **AI-powered gesture recognition**, and instantly converts it into **text and speech output**.

The platform focuses on **accessibility, inclusivity, and seamless human-computer interaction**, enabling users to communicate naturally using hand gestures without requiring specialized devices.

---

## **Problem Statement**

People who rely on sign language often face communication barriers in daily interactions due to limited understanding of sign language among the general public. Existing solutions may require complex setups or work poorly in varied environments.

**SWar solves this by providing:**

* Real-time gesture recognition
* Instant text conversion
* Voice output for spoken communication
* Easy camera-based interaction
* Fast and accessible UI

---

## **Key Modules**

### **1) Live Detection Module**

* Captures hand gestures using webcam
* Detects hand position in real-time
* Uses ROI (Region of Interest) box for stable recognition
* Ensures proper hand alignment for better prediction

### **2) Sign Recognition Engine**

* Recognizes:

  * **A–Z Alphabets**
  * **0–9 Numbers**
  * **Common Sentences / Gestures**
* Confidence-based prediction system
* Alternative prediction suggestions
* Stable-frame detection for accurate results

### **3) Text Conversion Module**

* Converts detected sign into readable text
* Maintains transcript history
* Allows sentence building from multiple signs

### **4) Voice Output Module**

* Uses speech synthesis
* Converts translated text into voice
* Enables natural communication

### **5) Learning / Gallery Module**

* Shows supported signs visually
* Helps users learn gestures
* Improves accessibility for beginners

### **6) User Interface Module**

* Interactive modern UI
* Live camera feed
* Detection feedback messages
* Responsive web design
* Theme support

---

## **Technology Stack**

### **Frontend**

* React + TypeScript
* Vite
* Tailwind CSS
* ShadCN UI

### **AI / Detection**

* TensorFlow.js
* MediaPipe Hand Landmarks
* Custom Geometric Sign Classifier

### **Browser APIs**

* Web Camera API
* Speech Synthesis API

---

## **Core Features**

✅ Real-time sign detection

✅ Sign → Text conversion

✅ Text → Voice conversion

✅ A–Z sign recognition

✅ 0–9 number recognition

✅ Fast prediction (<100ms latency)

✅ Live transcript panel

✅ Beginner-friendly sign gallery

✅ Responsive design

---

## **Objective**

The main objective of **SWar** is to create a **smart communication bridge** that transforms hand gestures into understandable speech and text, making communication more inclusive for individuals with hearing or speech disabilities.

---

## **Future Scope**

* Sentence auto-correction
* Regional language voice output
* Mobile app version
* Two-way communication mode (Voice → Sign)
* More gesture dataset expansion
* Personalized learning mode

---
