# 🛡️ PEShield – Malware Analysis Using Machine Learning

PEShield is a machine learning-based malware detection system that analyzes PE (Portable Executable) headers and URLs to classify files or links as malicious or benign. This project is part of an academic initiative in malware analysis and focuses on integrating lightweight, explainable models for practical malware detection on edge devices.

---

## 📖 About the Project

With the rise in cyberattacks through portable executable (PE) files and malicious URLs, PEShield leverages machine learning to improve malware classification accuracy using:

- **Static analysis** of PE headers extracted from Windows binaries
- **URL analysis** using Natural Language Processing techniques to detect patterns in malicious domains

The system includes two modules:

- **PE File Classifier**: Uses features like entropy, virtual size, and import functions extracted from PE headers
- **Malicious URL Detector**: Uses text-based patterns and NLP techniques (like TF-IDF) to classify URLs

The models are optimized for deployment on resource-constrained environments, aiming for real-time detection with minimal overhead.

---

## 🔧 Tech Stack

- **Programming Language**: Python 3.8+
- **Libraries**:
  - `pandas`, `numpy`, `matplotlib`, `seaborn`
  - `scikit-learn`, `joblib`
  - `pefile` – For extracting PE header fields
  - `nltk`, `re` – For URL preprocessing and analysis

- **Operating System**: Windows / Kali Linux
- **IDE**: Jupyter Notebook / VS Code

---

## 🚀 How to Run on Local Machine

### ✅ Prerequisites

- Python 3.8 or higher
- Git installed (optional but recommended)

### 📦 Installation Steps

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/peshield.git
   cd peshield
2. **Create a virtual environment (optional but recommended)**
   ```bash
   python -m venv venv
   source venv/bin/activate       # On Linux/Mac
   venv\Scripts\activate          # On Windows
3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
4. **Run**
   ```bash
   python main.py

📊 Features
ML-based static analysis without executing the malware

TF-IDF-based NLP model for suspicious URL detection

Whitelisting logic to reduce false positives in URL analysis

Support for model persistence using joblib

Accuracy:

PE File Detection: ~96%

URL Detection: ~92%

🧠 Research Context
This project draws on research that highlights the efficiency of static malware detection using lightweight classifiers. Unlike dynamic malware analysis, which requires execution in a sandbox, PEShield relies solely on header fields and URL strings—making it faster and safer for endpoint deployment. The project also considers model interpretability and memory footprint, suitable for edge devices and IoT environments.

📫 Contact
For questions or contributions, feel free to connect via GitHub Issues.
or contact : chaudharydivyanshi238@gmail.com
