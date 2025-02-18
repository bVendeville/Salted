# Salted: dataSet for the evALuation of simplificaTion Errors Detection

Welcome to **Salted**! This repository provides a comprehensive set of resources to evaluate errors in automatic text simplification. Here you will find our dataset, a detailed taxonomy of error types, an annotation scheme, and annotation templates—all designed to help you effectively identify and analyze simplification errors.

---

## Repository Contents

- **Dataset:**  
  A structured dataset containing original and simplified sentences along with detailed error annotations.  
  **File Format:** Typically provided as CSV or similar tabular formats.

- **Taxonomy:**  
  Our error taxonomy is available in both PNG and PDF formats. This visual and document-based taxonomy outlines the classification of simplification errors, including:
  - **Fluency Errors**
  - **Alignment Errors**
  - **Information Errors**
  - **Simplification Errors**  

- **Annotation Scheme:**  
  Detailed guidelines provided in a Microsoft Word document. This scheme explains the annotation procedures.

- **Annotation Templates:**  
  Excel (XLSX) files with clean headers. These templates are designed for annotators to paste each line of the dataset and mark errors according to the provided scheme.

---

## Dataset Description

The dataset is organized with the following columns and data types:

| **Column**                                     | **Data Type** | **Description**                                      |
|------------------------------------------------|---------------|------------------------------------------------------|
| **source sentence**                            | Object        | The original sentence before simplification.        |
| **simplified sentence**                        | Object        | The automatically simplified version.               |
| **run_id**                                     | Object        | Identifier for the simplification run of the participant.     |
| **snt_id**                                     | Object        | Unique sentence identifier.                         |
| **No error**                                   | Boolean       | Marks if no error is present.                       |
| **A1. Random generation**                      | Boolean       | Indicates random generation errors.                 |
| **A2. Syntax error**                           | Boolean       | Indicates syntactic errors.                         |
| **A3. Contradiction**                          | Boolean       | Indicates contradiction errors.                     |
| **A4. Simple punctuation / grammar errors**    | Boolean       | Indicates simple punctuation/grammar errors.        |
| **A5. Redundancy**                             | Boolean       | Indicates redundancy errors.                        |
| **B1. Format misalignment**                    | Boolean       | Indicates format misalignment errors.               |
| **B2. Prompt misalignment**                    | Boolean       | Indicates prompt misalignment errors.               |
| **C1. Factuality hallucination**               | Boolean       | Indicates factuality hallucination errors.          |
| **C2. Faithfulness hallucination**             | Boolean       | Indicates faithfulness hallucination errors.        |
| **C3. Topic shift**                            | Boolean       | Indicates topic shift errors.                       |
| **D1.1. Overgeneralization of Concepts**       | Boolean       | Indicates overgeneralization errors.                |
| **D1.2 Overspecification of Concepts**         | Boolean       | Indicates overspecification errors.                 |
| **D2.1. Loss of Informative Content**          | Boolean       | Indicates loss of informative content.              |
| **D2.2. Out-of-Scope Generation**              | Boolean       | Indicates out-of-scope generation errors.           |
| **Commentaire**                                | Object        | Additional comments regarding the annotation.       |
| **Annotator**                                  | Object        | Identifier of the annotator.                        |


---

## Getting Started

### Prerequisites
- **Python 3.12** (if you plan to run analysis scripts)
- Microsoft Excel or Google Sheets (for viewing/editing the XLSX templates)
- Microsoft Word or Google Docs (for the annotation scheme document)
- A PDF reader and image viewer (for the taxonomy documents)

### Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/bVendeville/Salted.git
   cd Salted
