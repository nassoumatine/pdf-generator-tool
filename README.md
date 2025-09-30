# 📄 PDF Notebook Generator

A simple Python tool that generates **lined PDF pages** from a list of topics in a CSV file.  
Each topic gets its own section with a **header, footer, and notebook-style lines**, making it perfect for study notes, journals, or custom printable notebooks.

---

## Features
- Reads topics and page counts from a `topics.csv` file.  
- Creates lined notebook pages for each topic.  
- Adds **headers** (topic name) and **footers** (topic name, small italic text).  
- Supports multiple pages per topic.  
- Outputs a clean, printable `output.pdf`.  

---

## Usage

### 1. Prepare your CSV file
Your `topics.csv` should look like this:

```csv
Topic,Pages
Math,3
Physics,2
Chemistry,4
```
- Topic → the subject/title for each section. 
- Pages → number of pages to generate for that topic.

### 2. Run the script
```bash
python app.py
```
This will generate a file named output.pdf in the project folder.

---

## Example Output
- Page 1: “Math” at the top, lined notebook-style page. 
- e 2 & 3: more “Math” pages with footer. 
- Page 4 & 5: “Physics” pages. 
- etc.

---

## Requirements
```bash
pip install fpdf pandas
```
- fpdf – PDF generation
- pandas – CSV handling

---

👩🏾‍💻 Built with Python, FPDF, and curiosity.