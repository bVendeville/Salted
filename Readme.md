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

| **Column**                                     | **Data Type** | **Description**                                                              |
|------------------------------------------------|---------------|------------------------------------------------------------------------------|
| **source sentence**                            | Object        | The original sentence before simplification.                               |
| **simplified sentence**                        | Object        | The automatically simplified version of the source sentence.               |
| **run_id**                                     | Object        | Identifier for the run of simplification.                                  |
| **snt_id**                                     | Object        | Unique sentence identifier.                                                |
| **No error**                                   | Boolean       | Marks if no error is present in the simplified sentence.                   |
| **A1. Random generation**                      | Boolean       | Indicates if the error is due to random generation.                        |
| **A2. Syntax error**                           | Boolean       | Indicates syntactic errors.                                                |
| **A3. Contradiction**                          | Boolean       | Flags contradictions between the source and simplified texts.              |
| **A4. Simple punctuation / grammar errors**    | Boolean       | Marks minor punctuation or grammar errors.                                 |
| **A5. Redundancy**                             | Boolean       | Indicates redundancy in the simplified text.                               |
| **B1. Format misalignement**                   | Boolean       | Flags formatting misalignments.                                            |
| **B2. Prompt misalignement**                   | Boolean       | Indicates misalignment with the prompt or instruction.                     |
| **C1. Factuality hallucination**               | Boolean       | Marks instances where non-factual content is generated.                    |
| **C2. Faithfulness hallucination**             | Boolean       | Indicates hallucinations affecting faithfulness to the source content.     |
| **C3. Topic shift**                            | Boolean       | Flags shifts in topic or content drift.                                    |
| **D1.1. Overgeneralization**                   | Boolean       | Indicates overgeneralization errors.                                       |
| **D1.2 Overspecification of Concepts**         | Boolean       | Marks cases where concepts are described in excessive detail unnecessarily.|
| **D2.1. Loss of Informative Content**          | Boolean       | Flags loss of important information during simplification.                 |
| **D2.2. Out-of-Scope Generation**              | Boolean       | Indicates generation of content that is out-of-scope relative to the source.|
| **Commentaire**                                | Object        | Additional comments regarding the annotation.                              |
| **Annotator**                                  | Object        | Identifier or name of the annotator.                                         |

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
