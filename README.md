# AI VR Tutor  

An interactive AI-powered tutor designed to provide immersive learning experiences in **Virtual Reality (VR)**. The AI tutor is **pre-trained on user-supplied PDF documents** and enables users to engage in dynamic, speech-driven learning sessions. By combining **VR, Natural Language Processing (NLP), and Speech Recognition**, this system enhances user engagement and makes learning more interactive.  

---

## 📌 Table of Contents  
- [Introduction](#introduction)  
- [Technologies Used](#technologies-used)  
- [What is our AI VR Tutor?](#what-is-our-ai-vr-tutor)  
- [Pros & Cons](#pros--cons)  
- [Model Architecture](#model-architecture)  
- [Getting Started](#getting-started)  
- [Installation](#installation)  
- [Troubleshooting & Support](#troubleshooting--support)  
- [License](#license)  
- [Citation](#citation)  

---

## 📖 Introduction  

For this GitHub project, we developed an **AI VR Tutor** that can be trained on PDF text files and used to **teach users based on their specific source material**. The tutoring experience takes place in **VR**, making learning more **engaging and interactive** by simulating a real tutoring environment.  

---

## 🔧 Technologies Used  

### **Text Processing & AI Model**  
- **[Ollama](https://ollama.ai/)** – The runtime environment for executing the AI model.  
- **[Mistral (LLM)](https://mistral.ai/)** – A lightweight and efficient large language model used for generating responses.  
- **[Nomic Embed Text](https://github.com/nomic-ai/nomic-embed)** – Used for text embeddings, improving context understanding and retrieval.  

### **Speech Processing**  
- **[Whisper (OpenAI)](https://github.com/openai/whisper)** – Converts spoken input into text using a small English STT model.  
- **[TTS (Text-to-Speech)](https://coqui.ai/)** – Uses the Tacotron2 model for generating speech output from text.  
- **[SoundDevice](https://python-sounddevice.readthedocs.io/) & [SciPy](https://scipy.org/)** – For recording and handling audio files.  

---

## 🎓 What is our AI VR Tutor?  

Our **AI VR Tutor** is an **interactive learning assistant** that allows users to **upload PDFs** and receive tutoring based on the content. The AI **processes text, understands context, and provides explanations** using advanced **language models**.  

The tutoring session takes place in **Virtual Reality (VR)** to **increase engagement** and provide an experience similar to real-life tutoring. Users can **speak naturally** with the tutor, thanks to **speech-to-text (STT) and text-to-speech (TTS) integration**.  

### **Key Features:**  
✔ **Customizable AI Learning** – Users upload PDFs, and the AI tailors its knowledge accordingly.  
✔ **VR-Optimized Interaction** – Provides a fully immersive tutoring experience.  
✔ **Speech Recognition & Synthesis** – Enables natural voice-based communication.  
✔ **AI-Powered Explanations** – Ensures relevant and contextual answers.  
✔ **Flexible Use Cases** – Suitable for students, self-learners, and professionals.  

---

## ⚖️ Pros & Cons  

### ✅ **Pros:**  
✔ **Personalized Learning** – Custom AI tutoring based on user-provided materials.  
✔ **Immersive Engagement** – VR enhances focus and learning retention.  
✔ **Speech Integration** – Allows natural voice communication.  
✔ **Efficient Knowledge Retrieval** – AI quickly summarizes and explains concepts.  
✔ **Flexible Applications** – Usable in various educational settings.  

### ❌ **Cons:**  
✖ **Hardware Requirement** – Requires a **VR setup**, limiting accessibility.  
✖ **Processing Power** – Running AI in VR may require a **high-performance PC**.  
✖ **Training Time** – Initial setup and training can take time.  
✖ **Potential Misinformation** – AI accuracy depends on the quality of input PDFs.  

---

## 🏗️ Model Architecture  

*(Reference the models we have used in the project and  . Include diagrams or flowcharts if needed.)*  

---

## 🚀 Getting Started  

### **How to Setup**  
*(Explain how users can install dependencies, set up the VR environment, and prepare training data.)*  

### **Training & Testing**  
*(Guide users on training the model, assessing results, and improving performance.)*  

---

## 🛠️ Installation  

### **Prerequisites**  
- Python **3.12.0**  
- Required Python libraries:  

### **Install Required Dependencies:**  
```sh
pip install -r requirements.txt

<details>
  <summary><h2>Project Setup</h2></summary>

  <details>
    <summary><h3>Windows Setup</h3></summary>

  To run the complete project with the correct dependencies, you first need to install a package manager. Follow the instructions to install [Chocolatey](https://docs.chocolatey.org/en-us/choco/setup/).Normally it is something like:

  For cmd.exe:
  ```bash
  @"%SystemRoot%\System32\WindowsPowerShell\v1.0\powershell.exe" -NoProfile -InputFormat None -ExecutionPolicy Bypass -Command "[System.Net.ServicePointManager]::SecurityProtocol = 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))" && SET "PATH=%PATH%;%ALLUSERSPROFILE%\chocolatey\bin"
  ```
  For powershell.exe:
  ```bash
  Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))
  ```

  Then install `make`:

  ```bash
  choco install make
  ```

  Once installed you can simply run:

  ```bash
  make setup
  ```

  And then:

  ```bash

  make python_deps

  ```
  </details>


  <details><summary><h3>MacOs Setup</h3></summary>


  This will install for `MacOs` users [homebrew](https://brew.sh/) and [uv](https://docs.astral.sh/uv/).If you already have a package manager and `uv` already installed,to be able to have all of the required dependencies run:

  ```bash 
  make setup
  ```
And for the dependencies:

  ```bash
  make python_deps
  ```
  or the same:

  ```bash
  uv sync
  ```
</details>
</details>


  If an enviroment existed already it will update the dependencies. If one did not exist, it will create it and populate it.
  Check [uv documentation](https://docs.astral.sh/uv/getting-started/features/) for more information

---

## 🛠️ Troubleshooting & Support  

If you encounter any issues, try the following solutions:  

### **Common Issues & Fixes**  

- ❌ **Python version mismatch** – Ensure you're using **Python 3.10+**.  
- 🎧 **No sound detected** – Check microphone permissions and ensure it's properly connected.  
- 🖥️ **VR environment crashes** – Update your **GPU drivers** and ensure your VR software is up-to-date.  
- ⚠️ **AI tutor doesn't recognize speech** – Make sure the **Whisper model** is installed and properly loaded.  
- 📁 **Training data not loading** – Ensure your **PDF files** are in the correct format and directory.  

### **Additional Help**  

- Check out the **[Issues section](https://github.com/your-repo/issues)** for known problems and solutions.  
- Join our **[Discord Community](https://discord.gg/Ujz8kNuZ)** for real-time support.  
- If all else fails, **open a new issue** on GitHub with a detailed error report.  

---

## 📜 License  

This project is licensed under the **[GNU Affero General Public License (AGPL v3)](https://www.gnu.org/licenses/agpl-3.0.html)**. See the **[LICENSE](https://github.com/your-repo/LICENSE)** file for details.  

---

## 📚 Citation  

If you use this project in your research or development, please cite it as follows:  

### **BibTeX Citation Format**  
```bibtex
@article{AIVRTutor2025,
  author = {Your Name(s)},
  title = {AI VR Tutor: Interactive Virtual Reality Learning with AI},
  year = {2025},
  journal = {GitHub Repository},
  url = {https://github.com/Data-Science-and-Society-2026/simulation_exercise/tree/master}
}
```

### **APA Citation Format**  
> Your Name(s). (2025). *AI VR Tutor: Interactive Virtual Reality Learning with AI*. GitHub Repository. Retrieved from [https://github.com/Data-Science-and-Society-2026/simulation_exercise/tree/master)  

---
