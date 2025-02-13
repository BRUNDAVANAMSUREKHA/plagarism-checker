# Plagiarism Checker

This is a Flask-based web application that allows users to check documents for plagiarism. Users can sign up, log in, and upload text or documents to analyze their originality. The system integrates advanced Natural Language Processing (NLP) models to enhance plagiarism detection, inspired by recent research on semantic analysis and AI-generated content detection.

## Outcome
Welcome to the **Plagiarism Checker-Login Page**, where users can securely access their accounts to utilize our powerful plagiarism detection features.

### **What You Will See on This Page:**
- **Login Form** – Enter your username and password to log in.
- **Signup Option** – New users can switch to the signup tab to create an account.
- **Secure Authentication** – Your credentials are encrypted for security.
- **User-Friendly Interface** – A simple, intuitive design for seamless navigation.

Once logged in, you will gain access to our **plagiarism detection tools**, where you can upload documents, analyze content originality, and receive a detailed plagiarism report.

![image](https://github.com/user-attachments/assets/153201ca-3076-4abb-884a-c99b8c6a6252)

Welcome to the **Plagiarism Checker-Results Page**, where you can review a detailed analysis of your submitted document. Our system utilizes advanced **Natural Language Processing (NLP) models** to provide an in-depth plagiarism report.

### **What You Will See on This Page:**
- **Plagiarism Score** – A percentage indicating the originality of your document.
- **Matched Sources** – List of external sources where similarities were detected.
- **Visual Reports** – Interactive charts and indicators to help you understand content overlap.
- **Content Breakdown** – Segmentation of plagiarized vs. original content for better insights.

By leveraging state-of-the-art models like **multi-qa-mpnet-base-dot-v1, roberta-large-openai-detector, and xlm-roberta-large**, our system ensures precise **semantic similarity detection, AI-generated content identification, and multilingual analysis**.
 ![image](https://github.com/user-attachments/assets/c3e16460-bfd9-418d-88fa-6a17322d83d1)
🔹For text input
![image](https://github.com/user-attachments/assets/463d59da-9939-42e9-80d2-fc988b21da9f)
🔹Results of the text given 
![image](https://github.com/user-attachments/assets/7ccec741-ba11-4865-a2fc-80d2ca477eae)
🔹 ![image](https://github.com/user-attachments/assets/98824626-e5f6-46fd-b991-4072bebdf485)
🔹for uploadding doecument
![image](https://github.com/user-attachments/assets/8dcb0dac-05bd-4f6e-9387-3a72d4e6bfa9)
🔹 ![image](https://github.com/user-attachments/assets/8a0c2286-6276-408a-9539-6672d8eea462)
🔹Results of the uploaded document
![image](https://github.com/user-attachments/assets/efec3056-679b-4459-bb98-ccfe46c26841)

## Features
- User authentication (Signup & Login)
- File upload support (.txt, .pdf, .docx)
- Advanced NLP-based plagiarism detection
- AI-generated content identification
- Multilingual plagiarism analysis
- Database storage for users, documents, and results
- Interactive UI with real-time feedback

## Technologies Used
- **Backend:** Flask (Python)
- **Frontend:** HTML, CSS, JavaScript
- **Database:** MySQL
- **Security:** Password hashing using `werkzeug.security`
- **Machine Learning Models:** `multi-qa-mpnet-base-dot-v1`, `roberta-large-openai-detector`, `xlm-roberta-large`

## Installation
### Prerequisites
Ensure you have the following installed on your system:
- Python (>=3.6)
- MySQL Server
- Pip (Python package manager)

### Setup Instructions
1. Clone the repository:
   ```sh
   git clone https://github.com/your-repo/plagiarism-checker.git
   cd plagiarism-checker
   ```
2. Install dependencies:
   ```sh
   pip install -r requirements.txt
   ```
3. Configure the MySQL database:
   - Create a MySQL database named `plagiarism`.
   - Update database credentials in `app.py` under the `query_db` function.
   - Run the provided SQL script (if available) to create necessary tables.

4. Run the application:
   ```sh
   python app.py
   ```
5. Open your browser and go to:
   ```
   http://127.0.0.1:5000/
   ```

## Project Structure
```
plagiarism-checker/
│── static/
│   ├── js/
│   │   ├── plagiarismDetector.js
│   │   ├── app.js
│   ├── images/
│── templates/
│   ├── home.html
│   ├── plagiarism.html
│── database/
│   ├── plagiarism.sql
│── uploads/  # Stores uploaded documents
│── app.py  # Main Flask application
│── requirements.txt  # Dependencies
│── README.md  # Project documentation
```

## Usage
1. Open the application in your browser.
2. Sign up for a new account.
3. Log in using your credentials.
4. Upload a document or input text manually.
5. Click "Analyze" to get plagiarism results.
6. View the plagiarism score and matched sources.

## Research-Based Enhancements
Based on the research paper on plagiarism detection using NLP models, the following advanced features have been incorporated:
- **Semantic Similarity Detection:** Uses `multi-qa-mpnet-base-dot-v1` to detect paraphrased text.
- **AI-Generated Content Identification:** Leverages `roberta-large-openai-detector` to spot AI-generated text.
- **Multilingual Support:** `xlm-roberta-large` enables plagiarism detection across multiple languages.
- **Comprehensive Reports:** Provides detailed plagiarism scores, matched sources, and visual indicators for better user understanding.

## License
This project is licensed under the MIT License.
