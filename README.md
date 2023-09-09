## Installation

First, clone project from repo:

```bash
# run
git clone https://github.com/erkartik2001/GPT-Doc-Chatbot.git
```


Install with pip:

```bash
# run
$ pip install -r requirements.txt
```


Create ``` .env``` file.


Add ``` PINECONE_API_KEY=ENTER_YOUR_PINECONE_KEY ``` in .env file.


Run the development server:

```bash
# run
python main_beta.py
```


App will be served on [http://127.0.0.1:5000](http://127.0.0.1:5000)

Add url to frontend ``` NEXT_PUBLIC_API_URL=ENTER_YOUR_BACKEND_URL ``` in .env file.

## For Production

Install:

```bash
# run
pip install gunicorn eventlet
```

Run command to start server:

```bash
# run
gunicorn -k eventlet -w 1 main_beta:app
```
