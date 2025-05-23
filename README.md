# PrattDeepResearch

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

An automated research tool that leverages LLMs and web search to generate comprehensive academic reports on any topic.

## 🔍 Overview

PrattDeepResearch is an AI-driven research automation pipeline that combines the power of large language models (LLMs) and web search to create well-structured academic reports. The system handles the entire research workflow:

1. **Planning**: Automatically creates a detailed research plan with specific questions
2. **Information Gathering**: Searches the web for relevant information using the Exa API
3. **Evaluation & Refinement**: Critically assesses research quality and identifies knowledge gaps
4. **Report Generation**: Produces a well-formatted academic report with proper citations

## ✨ Features

- **Multi-agent Architecture**: Uses specialized LLM agents for each stage of the research process
- **Comprehensive Web Search**: Leverages Exa for high-quality search results and content retrieval
- **Critical Evaluation**: Identifies research gaps and automatically pursues additional information
- **Academic Formatting**: Generates properly structured academic content with references
- **Persistent Storage**: Saves completed research as Markdown files

## 🛠️ Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/PrattDeepResearch.git
cd PrattDeepResearch

# Install required packages
pip install exa-py langchain langchain-openai python-dotenv
```

## Or access the code example on Google Colab
https://colab.research.google.com/drive/17sUvC5r1BfYv5QRth0vn44gBuyoeT5fi#scrollTo=Yb0ZlytAb2g7

## 🔑 API Keys Setup

The tool requires the following API keys, you can request these API keys via OnePratt - https://one.pratt.edu/s/contactsupport :
1. **Exa API**: For web search capabilities
2. **OpenAI API**: For access to GPT models

Create an `env.txt` file with the following contents:
```
EXA_API_KEY=your_exa_api_key_here
OPENAI_API_KEY=your_openai_api_key_here
```

## 🚀 Usage

The tool is provided as a Jupyter notebook (`deepResearch.ipynb`). Load it in your preferred environment:

```python
# After setting up API keys, run a research pipeline
topic = "Compare the recent marketing strategy between Coca Cola and Pepsi"
run_research_pipeline(topic)
```

This will:
1. Create a detailed research plan
2. Gather information from the web
3. Evaluate and refine the research
4. Generate a complete academic report
5. Save the report as a Markdown file

## 📋 Pipeline Components

- **Planning Agent**: Creates a structured research plan (uses o3-mini)
- **Researcher Agent**: Executes web searches and synthesizes information (uses GPT-4.1)
- **Evaluator Agent**: Assesses research quality and identifies gaps (uses GPT-4.1)
- **Writer Agent**: Formats findings into academic text with references (uses GPT-4.1)

## 📄 Output

The system generates a Markdown file containing:
- The original research topic
- Evaluation of the research quality
- A comprehensive research report
- References with source URLs

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📝 License

This project is licensed under the MIT License - see the LICENSE file for details.

## ✉️ Contact

For questions or feedback, please open an issue on this repository.

---

*Note: This tool is for academic and research purposes only. Always verify information and citations generated by AI systems.*