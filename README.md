# Quickstart

## Context
I studied science and engineering at university. I still read some publications from time to time, and on top of that I am an avid reader of non-fiction and news. It's safe to say that a lot of information goes through my mind. Luckily for me, the knowledge doesn't just enter through one ear and, immediately, leave through the other. I sometimes have the oppoturnity to bring it up in conversation with people. However, even in those cases where the ideas are fresh, some parts can escape me. I can't tell you how frustrating it is to try and go through my search history — especially with the updates Google brought to chrome :( — and physical books to find that one paragraph you vaguely remember reading.

The idea for Libby comes from that annoyance. Libby is your own second brain. A more robust and expansive one. Libby learns from your search history and answers your natural language questions about that inane article you read when you were waiting for a latte at your favorite coffee spot.

## Setup

1. If you don’t have Python installed, [install it from here](https://www.python.org/downloads/)

2. Clone this repository

3. Navigate into the project directory

   ```bash
   $ cd openai-quickstart-python
   ```

4. Create a new virtual environment

   ```bash
   $ python -m venv venv
   $ . venv/bin/activate
   ```

5. Install the requirements

   ```bash
   $ pip install -r requirements.txt
   ```

6. Make a copy of the example environment variables file

   ```bash
   $ cp .env.example .env
   ```

7. Add your [API key](https://beta.openai.com/account/api-keys) to the newly created `.env` file

8. Run the app

   ```bash
   $ flask run
   ```

You should now be able to access the app at [http://localhost:5000](http://localhost:5000)!

## Further Work
The Jupyter Notebook trains OpenAi's GPT3 model on an interview of Tony Fadell by Tim Ferriss. The model is able to answer questions, but only ones that match (word for word) the ones in the fine-tuning dataset. The model also tends to answer questions based on its base training instead of the fine-tune.

Here are some suggestions for further work:
1. Making the model answer questions with different formulations to the ones in the fine-tuning dataset.
2. Making the model go through it's fine-tuned knowledge before its base knowledge.
