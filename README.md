# Cold Email Generator

The **Cold Email Generator** is an intelligent system designed to automate the creation of personalized cold emails for job applications. By analyzing a given job description, the system matches the required skills and qualifications with relevant portfolio links and metadata, generating a tailored email that aligns with the job profile. This project leverages cutting-edge AI models and a robust vector database for efficient and accurate results.

---

## Key Features

- **AI-Powered Email Generation**: Uses the **Llama 3.1 API** trained on 70 billion parameters to generate highly personalized and contextually accurate cold emails.
- **Vector Database Integration**: Implements **ChromaDB** to store and retrieve portfolio links and metadata based on skill and qualification matches.
- **Automated Matching**: Dynamically matches the job description's requirements with stored data for precise recommendations.
- **Scalability**: Capable of handling a wide range of job descriptions across industries and domains.

---

## Project Workflow

1. **Input Job Description**: Users provide a job description.
2. **Skill and Qualification Matching**:
   - The system queries **ChromaDB** to retrieve relevant portfolio links and metadata.
   - Matching is based on skills and qualifications specified in the job description.
3. **Cold Email Generation**:
   - The **Llama 3.1 API** processes the input and matched data to create a personalized email.
   - The email highlights the candidate's strengths, qualifications, and portfolio links, tailored to the job profile.
4. **Output**: The generated email is presented to the user for further customization or direct use.

---

## Technologies Used

- **Programming Language**: Python
- **AI Model**: Llama 3.1 API (70 billion parameters)
- **Database**: ChromaDB (Vector Database)
- **Libraries and Frameworks**:
  - `pandas` for data manipulation
  - `numpy` for numerical computations
  - `llama-api` for interacting with the Llama 3.1 API
  - `chromadb` for vector database operations

---

## Installation

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/cold-email-generator.git
   cd cold-email-generator
   ```
2. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
   ```
   Ensure you have Python 3.8 or later installed.

3. **Set Up API Keys**:
   - Obtain an API key for the Llama 3.1 API.
   - Add it to a `.env` file:
     ```
     LLAMA_API_KEY=your_api_key_here
     ```

4. **Configure ChromaDB**:
   - Ensure ChromaDB is running and configured to store and retrieve metadata.

---

## Usage

1. **Run the Application**:
   ```bash
   python main.py
   ```
2. **Provide Job Description**: Input the job description as prompted.
3. **Receive Generated Email**: The system will output a customized cold email.

---

## Example Output

**Input Job Description**:
```
Looking for a Software Engineer proficient in Python, Machine Learning, and Cloud Platforms. Must have experience with data pipelines and deployment.
```

**Generated Cold Email**:
```
Subject: Application for Software Engineer Position

Dear [Hiring Manager's Name],

I hope this email finds you well. My name is [Your Name], and I am thrilled to apply for the Software Engineer position at [Company Name]. With extensive experience in Python, Machine Learning, and Cloud Platforms, I have successfully designed and deployed robust data pipelines that drive impactful solutions.

I have attached my portfolio showcasing projects like [Project 1] and [Project 2], highlighting my expertise in [specific skills]. I am confident that my skills align perfectly with your requirements and would love to contribute to your team's success.

Thank you for considering my application. I look forward to the opportunity to discuss how my experience can benefit [Company Name].

Best regards,
[Your Name]
```

---
