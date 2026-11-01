# NLP lab solutions

Each folder, `lab1` through `lab11`, contains a `solution.ipynb` notebook with answers to the tasks in its linked guidelines.

## Setup

Use Python 3.12:

```sh
python3.12 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
python -m spacy download en_core_web_sm
```

Open a notebook in Jupyter or VS Code, select this environment, and run all cells from its lab folder. The first run downloads NLTK resources, Kaggle datasets, and Hugging Face model weights as needed; internet access is required. Labs 5, 6, and 11 include the datasets supplied with the guidelines. Kaggle downloads stay in the local cache.

Lab 4 uses the full Amazon review dataset and may take several minutes. Lab 5 trains Word2Vec on all supplied Simpsons dialogue. Models use a fixed seed where practical; generated text in Lab 7 intentionally uses random sampling.

Lab 9 asks for a sentence and saves its trained model to `lab9/custom_ner_model/`. Lab 10 trains a small English–French LSTM on 10,000 short sentence pairs; it demonstrates the method rather than providing reliable e-commerce translations. Lab 11 visualizes attention on the supplied training questions, so its reported accuracy is training accuracy.

