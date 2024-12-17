# Multiple RAGs: Retrieval-Augmented Generation with Multiple Data Sources

This repository demonstrates an implementation of **Multiple RAGs (Retrieval-Augmented Generation)** for building AI systems that efficiently query multiple data sources and generate contextual responses. The project supports two key use cases:

1. **URL-based RAG**: Retrieves and processes content from web pages to provide relevant answers.
2. **PDF-based RAG**: Loads, processes, and queries PDF documents for contextual information retrieval.

The project utilizes a Colab notebook for easy execution and experimentation.

## Features
- Combines retrieval-based techniques with language generation.
- Leverages powerful libraries such as **LangChain**, **Unstructured**, **PyMuPDF**, and **HuggingFace**.
- Supports integration of multiple knowledge bases or data sources.
- User-friendly notebook-based implementation for rapid prototyping.

---

## How to Use

### 1. Clone the Repository

First, clone the repository to your local machine:
```bash
git clone https://github.com/dsaidinesh/multiple_rags.git
cd multiple_rags
```

### 2. Load the Notebook into Google Colab

#### Option A: Direct Upload
1. Download the `main.ipynb` file from the repository.
2. Go to [Google Colab](https://colab.research.google.com/).
3. Click on **File > Upload Notebook** and select the `main.ipynb` file.

#### Option B: Open from GitHub
1. Navigate to [Google Colab](https://colab.research.google.com/).
2. Click on **File > Open Notebook > GitHub**.
3. Paste the repository link: `https://github.com/dsaidinesh/multiple_rags`.
4. Select the `main.ipynb` notebook and click **Open Notebook**.

#### Option C: Use Google Drive
1. Upload the `main.ipynb` file to your Google Drive.
2. Open [Google Colab](https://colab.research.google.com/) and connect your Drive.
3. Navigate to the uploaded notebook and open it in Colab.

---

### 3. Execution Steps

The notebook walks through the following major steps:
1. **Install Dependencies**: The necessary libraries are installed using pip commands:
   ```python
   pip install langchain langchain_community unstructured langchain-chroma
   pip install langchain-text-splitters==0.2.2 langchain-huggingface==0.0.3 unstructured==0.15.0 nltk==3.8.1
   pip install pymupdf
   ```

2. **Import Libraries**: Essential modules such as `langchain`, `PyMuPDFLoader`, and `CharacterTextSplitter` are loaded.

3. **Document Loading**: Use `PyMuPDFLoader` to read and process PDF documents efficiently.

4. **Text Splitting**: Segment text using `CharacterTextSplitter` for downstream tasks.

5. **Embedding Creation**: Leverage `HuggingFaceEmbeddings` to create vector representations of the text.

6. **Query and Generate**: Combine retrieval and generation capabilities to create context-aware responses.

---

### 4. Alternatives to Colab

#### Jupyter Notebook
If you prefer running the notebook locally:
1. Install Jupyter Notebook:
   ```bash
   pip install notebook
   ```
2. Install required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Launch the notebook:
   ```bash
   jupyter notebook main.ipynb
   ```

#### VSCode with Jupyter Extension
1. Open the repository in VSCode.
2. Ensure the Jupyter extension is installed.
3. Open `main.ipynb` and execute the cells.

---

## Dependencies
To ensure smooth execution, the following dependencies are required:
- Python 3.8+
- Jupyter Notebook or Google Colab
- Libraries:
  - `langchain`
  - `unstructured`
  - `PyMuPDF`
  - `HuggingFace` modules
  - `nltk`

Install them via:
```bash
pip install -r requirements.txt
```

---

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## Contributions
Feel free to open issues or submit pull requests for enhancements or bug fixes!

---

## Contact
For any queries or support, reach out to:
- **Sai Dinesh**
- GitHub: [dsaidinesh](https://github.com/dsaidinesh)

Happy Coding!
