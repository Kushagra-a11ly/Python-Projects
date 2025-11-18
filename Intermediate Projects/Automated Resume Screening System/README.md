Automated Resume Screening System

This project is an automated tool that screens multiple resumes against a given job description using NLP, cosine similarity, and skill matching.
It extracts text from PDF/DOCX resumes, cleans the data, compares them with the job description, identifies required skills, and ranks all candidates.

📌 Features

Extracts text from PDF and DOCX resumes
Removes stopwords and cleans text using NLTK
Computes similarity between resumes and job description using
CountVectorizer + Cosine Similarity
Identifies matched skills between resume and job requirements
Generates a clean ranking of all candidates
Exports results to Excel (resume_ranking.xlsx)

📁 Project Structure
│── Automated Resume Screening System.py                     # Main script
│── README.md                                                # Documentation
│── resume_ranking.xlsx                                      # Auto-generated output
│── resumes/                                                 # Folder containing candidate resumes

⚙️ How It Works
Enter the folder path of resumes when prompted.
The script reads each file (.pdf or .docx).
Text is cleaned using NLTK stopwords.
A similarity score is calculated for each resume.
Skills are matched between resume and job description.
Results are sorted and displayed.
Output is exported to Excel.


📌 Required Libraries
Install dependencies before running:
pip install PyPDF2 python-docx nltk pandas scikit-learn
Download stopwords (only first run):
nltk.download('stopwords')

▶️ How to Run
Place resumes in a directory, for example:
resumes/
    candidate1.pdf
    candidate2.docx
    candidate3.pdf

Run the script:
python main.py
Enter the resume folder path:
Enter the path to the folder containing resumes: resumes
The ranked output appears on the terminal and is saved as:
resume_ranking.xlsx
