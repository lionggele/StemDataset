# Introduction: Simplifying Dataset Preparation from Hard Copy Questions

This workflow is designed to help you transform questions from physical materials (like books or PDFs) into a well-organized digital dataset. Whether you're working with scanned documents or PDF files, this process ensures that the data is cleaned, structured, and ready for use without requiring advanced technical knowledge.

By using tools like **Tesseract-OCR** and **EasyOCR**, you can extract text accurately from images or PDFs. Additionally, **PyMuPDF** helps process PDF files efficiently. The steps are easy to follow, even for beginners, making it ideal for creating datasets on platforms like Kaggle.

---

## Workflow Overview

### **Step 1–4: Question Cropping Workflow**

1. **PDF to Image Conversion**  
   - Convert each page of the PDF into an image.  
   - This step simplifies processing and helps in removing parts you don’t need, such as headers or footers.

2. **Removing Unnecessary Sections**  
   - Identify and eliminate redundant parts like repeated titles or sections (e.g., "Kertas 2").  
   - This ensures the dataset is focused on relevant questions.

3. **Tag Cleanup**  
   - Detect and remove irrelevant tags or extra text that might clutter your dataset.

4. **Column & Question Cropping**  
   - Split pages formatted in multiple columns (e.g., two or three columns).  
   - Process each column separately to ensure clean and organized extraction of questions and content.

---

### **Step 5: Answer Extraction Workflow**

5. **Answer Extraction**  
   - Use OCR tools (like EasyOCR or Tesseract) to automatically detect and extract answer keys or solutions from the images.  
   - Save extracted answers in a structured format (e.g., JSON), ensuring both question and answer data are preserved for further analysis.

---

### **Step 6–7: Dataset Consolidation Workflow**

6. **Combine Questions and Answers**  
   - Merge the datasets containing questions and answers into a unified JSON file.  
   - Each entry in the JSON file will include fields for the question, its associated answer, and any relevant metadata (e.g., page or section number).

7. **Export to Final Dataset**  
   - Convert the consolidated JSON file into a user-friendly format (e.g., `.csv` or `.xlsx`).  
   - This final dataset can be used for reviewing, sharing, or additional machine learning tasks.

---

## Summary of Outputs

- **Step 1–4**: A set of cropped images containing only relevant questions, saved as PNG files.  
- **Step 5**: A JSON file containing extracted answers, organized for each question.  
- **Step 6–7**: A consolidated dataset with questions and answers in JSON, then exported to `.csv` format for end users.
