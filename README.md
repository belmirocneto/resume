# Belmiro Neto - Resume

![Markdown](https://img.shields.io/badge/Markdown-validated-blue.svg?style=for-the-badge&logo=markdown&logoColor=white)
![PDF](https://img.shields.io/badge/PDF-Generated-brightgreen?style=for-the-badge&logo=adobeacrobatreader&logoColor=red)
![GitHub Actions](https://github.com/belmirocneto/resume/actions/workflows/convert-md-to-pdf.yml/badge.svg)

Welcome to my resume repository! This project contains my professional resumes in both **Portuguese (PT-BR)** and **English (EN)**. While contributions to improve **GitHub Actions automation** and repository workflows are welcome, **the content of the resume itself belongs to me**.

## 📄 Resumes

You can view my resumes in Markdown format:
- [Portuguese Version (PT-BR)](RESUME.md)
- [English Version (EN)](RESUME_EN.md)

## 🔒 Ownership & Usage

This resume is **my personal document**, and its content should not be altered except for **GitHub Actions automation improvements**. Any changes modifying personal details, experience, or professional background will not be accepted.

## 🚀 Contributing

I encourage contributions that enhance the **automation and CI/CD workflows** for generating and maintaining this resume. Possible improvements include:
- Enhancing the **GitHub Actions pipeline** for automatic PDF generation.
- Automating formatting checks or linting for Markdown files.
- Improving **workflow efficiency** for CI/CD processes.

### 📜 **GitHub Actions Workflow**  

This repository includes a **GitHub Actions workflow** that automatically converts `RESUME.md` and `RESUME_EN.md` into **PDFs** whenever changes are pushed.  

The workflow:  
✅ Uses **md-to-pdf** with **Puppeteer** for **accurate PDF rendering**.  
✅ Generates files as `pdf/RESUME-YYYYMMDD.pdf` and `pdf/RESUME_EN-YYYYMMDD.pdf`, based on the current date.  
✅ Automatically **commits the generated PDFs** back to the repository.  
✅ (Optional) **Sends an email with both latest resume PDFs** if Gmail credentials are configured.  

👀 **Ensure Workflow Permissions**: Verify that your repository's settings allow workflows to have write permissions:

   - Navigate to your repository on GitHub.
   - Click on the "Settings" tab.
   - In the left sidebar, select "Actions" and then "General".
   - Under "Workflow permissions", ensure "Read and write permissions" is selected.
   - Click "Save" to apply the changes.

You can find the workflow configuration in `.github/workflows/convert-md-to-pdf.yml`.  

### **📬 Email Notifications with Gmail**
Your **GitHub Actions workflow** includes an **optional feature** that automatically sends an email with your **latest resume PDFs** whenever `RESUME.md` or `RESUME_EN.md` is updated. 📄📩  

#### **🔹 How to Enable Email Sending**
1. **Generate a Gmail App Password**  
   - Go to [Google App Passwords](https://myaccount.google.com/apppasswords)  
   - Select **"Mail"** and generate a password  
   - Copy the **16-character password**  

2. **Set Up GitHub Secrets**  
   - Go to your **GitHub Repository → Settings → Secrets and Variables → Actions**  
   - Add the secrets:
     - **`GMAIL_USERNAME`** → Your Gmail (e.g., `your-email@gmail.com`)  
     - **`GMAIL_PASSWORD`** → Paste the **App Password**  

#### **🔹 Disabling Email Notifications**
- If you **do not set** `GMAIL_USERNAME` and `GMAIL_PASSWORD`, the email step will be **skipped** automatically.

## 📬 Contact

If you have any questions or suggestions, feel free to reach out:
- [LinkedIn](https://linkedin.com/in/belmiro-neto)
- [GitHub](https://github.com/belmirocneto)

## 👏 Credits & Acknowledgments

This repository is a fork of the original project created by [Luis Machado Reis](https://github.com/luismr/resume). 

The base structure and the GitHub Actions automation workflow for converting Markdown to PDF were adapted from his implementation.