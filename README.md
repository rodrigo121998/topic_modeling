# Topic modeling with AI 🤖📄

This repository contains a topic modeling with gen ai application that leverages the power of OpenAI's LLM model and Bertopic to cluster abstracts. You can give some abstracts and then clustering them

## Installation

1. Clone the repository to your local machine:

```bash
git clone https://github.com/rodrigo121998/topic_modeling.git
cd topic_modeling
```
2. Create a virtual environment with Python 3.10:
```bash
python3.10 -m venv venv
source venv/bin/activate
```
3. Install the required packages from the requirements.txt file:
```bash
pip install -r requirements.txt
```

## Usage

1. Activate the virtual environment:
```bash
source venv/bin/activate
```

2. In the `main.ipynb` is developed the topic modeling

3. You can load the model with this to get predictions
```python
# to load
# Define embedding model
embedding_model = SentenceTransformer("all-MiniLM-L6-v2")

# Load model and add embedding model
loaded_model = BERTopic.load("bertopic_model", embedding_model=embedding_model)
```

## Next steps
- Train with other variables to cluster
- Develop a self service app to get clusters