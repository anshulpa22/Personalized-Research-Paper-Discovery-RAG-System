# Personalized Research Paper Discovery RAG System

This project is a Google Scholar/ORCID-powered Research Paper Discovery system using Retrieval-Augmented Generation (RAG). It fetches recent papers relevant to your research profile, builds a vector database, and enables advanced querying and reporting.

## Features

- Extracts your research profile from ORCID
- Fetches recent papers from arXiv and mock IEEE/ACM sources
- Calculates relevance to your research interests
- Builds a RAG system with OpenAI, local, or keyword-based embeddings
- Supports personalized queries and generates research reports
- Exports results to BibTeX, CSV, JSON, and sets up an alert system

## Usage

1. **Install dependencies**  
   Run the following in a notebook cell:
   ```python
   !pip install langchain_community langchain_openai faiss-cpu openai scholarly arxiv requests beautifulsoup4 sentence-transformers scikit-learn
   ```

2. **Set your OpenAI API key**  
   Update the notebook cell for API key setup.

3. **Run the notebook**  
   Execute all cells in [Research_Paper_Assistance_RAG_System.ipynb](GenAI_Level2_Project_Submitted/Research_Paper_Assistance_RAG_System.ipynb).

4. **Exported files**  
   - `anshul_research_report.md`
   - `anshul_recent_papers.bib`
   - `anshul_recent_papers.csv`
   - `research_dashboard_data.json`
   - `alert_config.json`

## Example Queries

- `ask_anshul_assistant('What are the latest ML techniques for MIMO beamforming?')`
- `ask_anshul_assistant('Which conferences should I target for my 6G research?')`

## Advanced

- Modify keywords and relevance thresholds for custom recommendations.
- Integrate with your reference manager or set up weekly alerts.
