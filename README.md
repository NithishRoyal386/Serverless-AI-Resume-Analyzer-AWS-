# Serverless-AI-Resume-Analyzer-AWS


📌 Overview


The Serverless AI Resume Analyzer is a cloud-based application that analyzes resumes and provides an ATS-like score based on skills, keywords, and relevance. Built using AWS serverless architecture, this project demonstrates scalable, cost-efficient, and production-ready backend design. 


🎯 Key Features



📄 Resume text analysis with ATS-style scoring

🔍 Skill extraction and keyword matching

📊 Identification of missing skills

⚡ Fully serverless architecture (no server management)

🌐  HTTP API (via API Gateway) for fast and cost-efficient integration


🏗️ Architecture


Client (Postman / Frontend)
        ↓
API Gateway (/analyze endpoint)
        ↓
AWS Lambda (Processing Logic)
        ↓
Skill Matching + Scoring Engine
        ↓
JSON Response (Score + Insights)


🛠️ Tech Stack


Cloud Services

AWS Lambda – Backend compute

API Gateway (HTTP API) – Lightweight and low-latency API endpoint

IAM – Secure access control

Programming

Python (Core logic implementation)

Tools

POST /analyze (HTTP API)

Git & GitHub (Version control)


⚙️ How It Works


User sends resume text via API request

API Gateway triggers Lambda function

Lambda processes text:

Converts text to lowercase

Matches predefined skill keywords

Calculates ATS score

Returns structured JSON response


📥 API Usage


Endpoint

POST /analyze

Request Body


{

  "resume_text": "Your resume content here"

}

Sample Response

{

  "score": 70,
  
  "skills_found": ["java", "aws", "iot"],
  
  "missing_skills": ["python", "sql"]

}



🧠 Scoring Logic


Predefined skill set is used as reference

Score is calculated based on matched keywords

Missing skills are highlighted for improvement



🔐 Security & Best Practices


IAM roles used for secure service access

Serverless design reduces attack surface

No hardcoded credentials



💡 Why This Project?


Demonstrates real-world cloud architecture

Shows understanding of serverless computing

Implements practical ATS logic used in recruitment systems

Focuses on scalability, cost-efficiency, and performance



🚀 Future Enhancements


📄 PDF resume upload (S3 integration)

🤖 Advanced NLP using AI models

📊 Dashboard for visualization

🔗 Job description matching system


📌 Author


Nithish Royal Bandi


GitHub: https://github.com/NithishRoyal386

LinkedIn: https://www.linkedin.com/in/nithish-royal-798018249/



⭐ Conclusion 

This project highlights the ability to design and deploy a scalable cloud-native application using modern serverless technologies, making it highly relevant for 
roles in Cloud, DevOps, and Backend Engineering.




