# Rick and Morty Story Generator
[![Open in Streamlit](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://share.streamlit.io/e-tony/story_generator/main/app.py)

This project uses a [pre-trained GPT2 model](https://huggingface.co/gpt2), which was fine-tuned on [Rick and Morty transcripts](https://rickandmorty.fandom.com/wiki/Category:Transcripts), to generate new stories in the form of a dialog. The project uses Hugging Face's [Transformers library](https://github.com/huggingface/transformers) to do inference and [Streamlit](https://www.streamlit.io/) for the application. 


### Setup

This repository has only been tested with Python 3.7. 

Install the dependencies in a virtual environment:
```
python3.7 -m venv venv
source venv/bin/activate
pip install --upgrade pip setuptools
pip install -r requirements.txt
```

On the first run, the app will download the pre-trained model from Hugging Face's Model Hub or you can supply your own custom model in the `load_model()` function. To start the application, simply run:
```
streamlit run app.py
```
