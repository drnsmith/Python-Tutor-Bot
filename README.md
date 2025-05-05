# Python Tutor Bot

A Telegram-based AI-powered Python programming assistant that delivers daily lessons, interactive Jupyter/Colab notebooks, and auto-graded exercises. Perfect for building consistent, deliberate coding habits.

## Project Structure

```
python-tutor-bot/
├── README.md
├── bot.py                # Core bot logic (Telegram + OpenAI integration)
├── requirements.txt      # Python dependencies
├── lessons/
│   ├── templates/        # Prompt templates for lesson generation
│   └── tests/            # Pytest suites for auto-grading
├── notebooks/
│   └── template.ipynb    # Base Jupyter/Colab template
└── deploy/
    ├── Procfile         # For Heroku or similar
    └── Dockerfile       # Container setup
```

## Getting Started

1. **Clone the repository**

   ```bash
   git clone https://github.com/your-username/python-tutor-bot.git
   cd python-tutor-bot
   ```

2. **Install dependencies**

   ```bash
   pip install -r requirements.txt
   ```

3. **Configure environment variables**

   * `TELEGRAM_TOKEN`: Your BotFather token
   * `OPENAI_API_KEY`: Your OpenAI API key

4. **Run the bot locally**

   ```bash
   python bot.py
   ```

## Usage

* Send `/start` to your bot in Telegram to register and schedule your daily lesson at 19:00 (Pacific/Auckland).
* Reply with your code solution; the bot will auto-grade using the tests in `lessons/tests/`.
* Click the Colab link provided in the lesson to work in an interactive notebook.

## Development Roadmap

* **Phase 1**: Telegram-based delivery & auto-grading
* **Phase 2**: Slack integration option
* **Phase 3**: Web dashboard (Streamlit) for analytics & progress tracking

## Contributing

Feel free to open issues or submit pull requests. For major changes, please discuss via issue first.

## License

MIT © Natasha Smith

