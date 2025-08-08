#  Fake Certificate Detection

A **Streamlit** web application to analyze academic certificates and detect potential forgeries using **OCR** (Tesseract), **NLP** (spaCy), and heuristic rules.

---

##  Features
-  **File Upload**: Accepts JPG, PNG, and PDF certificates.
-  **OCR Text Extraction**: Reads certificate content with Tesseract.
-  **Suspicious Keyword Detection**: Flags terms often found in fake certificates.
-  **Missing Authentic Term Check**: Identifies absence of essential academic terms.
-  **Entity Recognition**: Extracts university names and degree mentions.
-  **Fake Score**: Calculates a 0–100 score indicating likelihood of authenticity.
-  **Interactive UI**: Displays document preview, extracted text, and detailed analysis.

---

##  Requirements
Before running the project, make sure you have:
- **Python 3.8+**
- **Tesseract OCR** installed
- **Poppler** (for PDF support)
- Internet connection (for downloading spaCy model)
- The following Python libraries:
  - streamlit  
  - pytesseract  
  - Pillow  
  - spacy  
  - PyMuPDF

## Run the application

streamlit run app.py 

## Example Output

Score ≥ 80 → Likely Genuine 

50 ≤ Score < 80 → Suspicious ⚠

Score < 50 → Likely Fake 
