# NLP lab solutions

Each folder, `lab1` through `lab7`, contains a `solution.ipynb` notebook with answers to the tasks in its linked guidelines.

## Setup

Use Python 3.12:

```sh
python3.12 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
python -m spacy download en_core_web_sm
```

Open a notebook in Jupyter or VS Code, select this environment, and run all cells from its lab folder. The first run downloads NLTK resources, Kaggle datasets, and Hugging Face model weights as needed; internet access is required. Labs 5 and 6 include the datasets supplied with the guidelines. Kaggle downloads stay in the local cache.

Lab 4 uses the full Amazon review dataset and may take several minutes. Lab 5 trains Word2Vec on all supplied Simpsons dialogue. Models use a fixed seed where practical; generated text in Lab 7 intentionally uses random sampling.

## Validation

All seven notebooks were executed from top to bottom with the pinned dependencies. Lab 4 achieved about 80% test accuracy; Lab 6 achieved 49%, so its classifier needs further work to become useful. The unsmoothed model in Lab 3 has infinite held-out perplexity for unseen bigrams, as explained in the notebook. Gensim completed Lab 5 with ignored `our_dot_float` warnings on macOS; these warnings remain visible in its saved outputs.
