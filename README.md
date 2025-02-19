# Rocket.Chat Docs Corpus
> Rocket.Chat Documentation Dataset

This repository contains a dataset extracted from the official [Rocket.Chat documentation](https://docs.rocket.chat/). The dataset is intended for research, machine learning, and other applications requiring structured documentation data.

## About
Rocket.Chat is an open-source communication platform that provides real-time chat, collaboration, and integrations. This dataset captures documentation content, including installation guides, API references, and feature explanations.

## Dataset Structure and Contents
This dataset is architected taking inspirations from [Databricks-dolly-15k HuggingFace Dataset](https://huggingface.co/datasets/databricks/databricks-dolly-15k/blob/main/databricks-dolly-15k.jsonl)

It includes:
- Extracted Content: Text and excerpts from Rocket.Chat documentation pages covering installation guides, API references, deployment instructions, and more.
- Multi-format Data: Structured records available in JSON, CSV, and Markdown formats to accommodate various processing and analysis pipelines.
- Rich Metadata: Information such as document titles, source URLs, and timestamps to provide context and traceability for each entry.
- Record Structure: Each record is composed of:
  - instruction: A prompt or question derived from the documentation.
  - context: Supplementary background information (when available) to enhance understanding.
  - response: The corresponding answer or explanation.
  - category: A label classifying the type of task (e.g., closed QA, open QA, classification, deployment).

This structured approach enables researchers and developers to fine-tune language models and build systems for enhanced documentation search, interactive chatbots, and automated content summarization tailored for Rocket.Chat.

## Usage
You can use this dataset for:
- Training NLP models for chatbot or search applications.
- Creating offline documentation.
- Analyzing changes in Rocket.Chat documentation over time.

## Example
```python
import pandas as pd

# Read the CSV file into a DataFrame
df = pd.read_csv('rocketchat_docs_qna.csv')

# Display the first few rows of the DataFrame
print("First 5 rows:")
print(df.head())
```

## Download
[Rocket.Chat Docs Dataset :arrow_down: ](https://raw.githubusercontent.com/r3yc0n1c/rocketchat-docs-corpus/refs/heads/main/rocketchat_docs_qna.csv)


## Contributing
Contributions are welcome! If you find any issues or want to improve the dataset, feel free to open an issue or submit a pull request.


## Contact

Have questions, suggestions, or ideas for modifications? Whether you need help with dataset formatting, scraping details, or have feedback on the corpus, we're here to help!

- Join the Community: [Chat](https://open.rocket.chat/channel/general)
- Report Issues or Ask Questions: [GitHub Issues](https://github.com/r3yc0n1c/rocketchat-docs-corpus/issues)

We welcome your feedback and contributions to help improve the dataset!
