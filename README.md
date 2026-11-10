# Restaurant Review Sentiment Classifier

A Streamlit app that classifies restaurant reviews as positive or negative.

## Run locally

Install the dependencies and start Streamlit:

```bash
pip install -r requirements.txt
streamlit run restaurent.py
```

Keep `output.csv` in the same directory as `restaurent.py`. It must have
`Review` and `Liked` columns, where `Liked` contains `0` or `1`.

## Deploy on Streamlit Community Cloud

The GitHub repository must contain these files at its root:

- `restaurent.py`
- `output.csv`
- `requirements.txt`

Then:

1. Push these files to the GitHub repository.
2. Sign in at [share.streamlit.io](https://share.streamlit.io/) with GitHub.
3. Select **Create app**, choose the repository and branch, and set the main
   file path to `restaurent.py`.
4. Select **Deploy**.

The app downloads the required NLTK corpora when it first loads the model.
