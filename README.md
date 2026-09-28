# HW4 starter: a tiny text generator

GLBL 5053 · Homework 4

`tiny_rnn.py` trains a very small neural network on ten short sentences and then generates new text one character at a time. You will run it, add comments to understand it, and track your work with Git.

## 1. Make your own copy

1. Near the top of this page, click **Use this template** → **Create a new repository**.
2. Owner: your GitHub account. Name: `hw4`, or anything you like. Visibility: **Private** is recommended. Your instructor will tell you how to share access.
3. Click **Create repository**. You now have your own repository, and your commits go there.

## 2. Clone it in VS Code

1. Open a new VS Code window and click **Clone Git Repository...**
2. Paste the link to *your* new repository (`https://github.com/<your-username>/hw4`), then choose a folder to put it in.
3. Open a terminal (**Terminal → New Terminal**), type `ls`, and press Enter. You should see `README.md`, `requirements.txt` and `tiny_rnn.py`.

## 3. Check your Python version

TensorFlow does not support the newest Python (3.14) yet. You need **Python 3.10–3.13**.

```
python3 --version
```

If it says 3.14 or later, install Python 3.13 from [python.org](https://www.python.org/downloads/) and use `python3.13` in the next step (on Windows, use `py -3.13`).

## 4. Create a virtual environment

- macOS/Linux:
  ```
  python3 -m venv .venv
  source .venv/bin/activate
  ```
  (Replace `python3` with `python3.13` if you installed it in step 3.)
- Windows (PowerShell):
  ```
  py -3.13 -m venv .venv
  .venv\Scripts\activate
  ```

If this worked, you will see `(.venv)` at the start of the line in your terminal.

## 5. Install TensorFlow

```
python -m pip install --upgrade pip
python -m pip install -r requirements.txt
```

This download is large, so it can take a few minutes.

## 6. Run the starter code

```
python tiny_rnn.py
```

It takes about a minute. TensorFlow prints some warning lines first; those are normal. At the end, you should see generated text like `I like puzzles.` at four different temperatures.

## If installing gets stuck

You can run the same file in [Google Colab](https://colab.research.google.com/), which already has TensorFlow: upload `tiny_rnn.py` using the folder icon on the left, then run `%run tiny_rnn.py` in a code cell. Keep committing your edits to your repository in VS Code as usual.
