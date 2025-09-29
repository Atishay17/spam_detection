Intelligent Threat Detection using AI in SOC
A next-generation email security system powered by Machine Learning, DistilBERT, and real-time Threat Intelligence APIs to detect spam, phishing, spoofing, and malicious attachments.

 Features:
 
1-Multi-class email classification (Ham, Spam, Promotions, Marketing, Phishing)
2-DistilBERT-powered text analysis for email content understanding
3-Real-time threat intelligence using:
4-Google Safe Browsing (malicious URL detection)
5-VirusTotal (attachment and URL scanning)
6-SPF, DKIM, DMARC (domain authentication checks)
7- SOC/SIEM-style dashboard for threat visibility
8-Gmail integration for real-time email fetching and analysis
9- Flask-based web interface for end-user interaction

 System Architecture:-

Email Fetching → Extracts headers, body, URLs, and attachments
Content Analysis → DistilBERT classifies emails into multiple categories
Threat Intelligence APIs → Validates URLs, scans attachments, and checks domain authenticity
Threat Scoring & Alerts → Generates threat scores and alerts for suspicious emails
Dashboard & UI → Flask web interface for monitoring results

## 📂 Project Structure  

```bash
📦 Intelligent-Threat-Detection
├── app.py                  # Flask main application
├── config.json             # Project configuration
├── credentials.json        # Gmail API credentials
├── fetch_gmails_OAuth.py   # Gmail fetch via OAuth
├── fetch_gmails_test.py    # Gmail fetching test script
├── fetch_gmails_test.cpython-312.pyc  # Compiled test script
├── index.html              # Main UI page
├── index.html.txt          # Backup HTML file
├── security_results.csv    # CSV log of classified emails & threats
├── special_tokens_map.json # Tokenizer special tokens mapping
├── tokenizer.json          # Trained tokenizer
├── tokenizer_config.json   # Tokenizer configuration
├── training_args.bin       # DistilBERT training args
├── vocab.txt               # Vocabulary file
├── vocab - Copy.txt        # Backup vocabulary
```

⚡ Tech Stack

Python (Flask, Pandas, NumPy, Requests)
Transformers (HuggingFace) – DistilBERT
APIs – Google Safe Browsing, VirusTotal
Email Security – SPF, DKIM, DMARC
Visualization – Dashboards & Reports

## 🔧 Installation & Usage  

Clone the repo  
```bash
git clone https://github.com/your-username/Intelligent-Threat-Detection.git
cd Intelligent-Threat-Detection
```
Install dependencies
```
pip install -r requirements.txt
```


Run Flask app
```
python app.py
```

```
[Open in browser
](http://127.0.0.1:5000/
)
```

📊 Results

✅ High accuracy spam/phishing classification with DistilBERT
✅ Real-time malicious URL & attachment detection
✅ End-to-end working SOC-inspired system with user-friendly dashboard

👨‍💻 Contributors:-

Atishay Jain – DistilBERT training, API integration, Flask UI (~70% contribution)
Harsh Arora – Data preprocessing, literature survey
Joel K Jose – Dashboard design, documentation

📜 References
Google Safe Browsing API
VirusTotal API
BERT Paper

Email Authentication (SPF/DKIM/DMARC)
✨ This project is part of academic research on next-generation email security and aims to bridge AI with real-time threat intelligence in SOC environments.
