# PDF_Content_Analysis_and_Question_Generation
Extracts text and images from PDFs and stores them in structured JSON format for AI-based question generation.

## 📄 PDF Content Analysis and Question Generation

### 🔍 Description

This Python project extracts **text** and **images** from a PDF file and generates a structured **JSON** file for question generation or content analysis.

---

### 🚀 Features

* Downloads a PDF from a given URL.
* Extracts text **page-by-page** using `pdfplumber`.
* Extracts all **images per page** using `PyMuPDF` (`fitz`).
* Stores the extracted data in a structured **JSON** format.
* Saves all images in an `output/images` folder.
* Zips the entire output directory for easy download.

---

### 🛠️ Requirements

Install dependencies:

```bash
pip install pdfplumber pymupdf requests
```

---

### 📁 Output Structure

```
output/
├── images/
│   ├── page1_option_image_1.png
│   ├── page2_option_image_1.png
│   └── ...
└── questions.json
```

**questions.json format:**

```json
[
  {
    "question": "Text content of page 1...",
    "option_images": [
      "output/images/page1_option_image_1.png"
    ]
  },
  ...
]
```

---

### 📌 Usage Steps

1. Install required packages.
2. Set your PDF download link in the code.
3. Run the script to extract text and images.
4. A zip file containing `questions.json` and all extracted images will be generated for download.

---

### 📦 Sample Output

* `questions.json`: Structured JSON with text and image paths.
* `output.zip`: Compressed folder containing all results.

---

### 👨‍💻 Author

Made by **Shashank Bhatt**
💡 Ideal for AI interns and ML developers working on PDF-based content extraction and understanding.

