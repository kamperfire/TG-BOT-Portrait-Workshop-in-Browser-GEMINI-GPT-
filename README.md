# Portrait Workshop Bot

Telegram bot for AI-assisted portrait generation, style presets, queue control, and browser-based creative workflows.

The project was built as a practical prototype for visual content automation: a user sends a photo, selects a style, and receives a generated portrait based on reusable prompt templates and a controlled generation flow.

## What It Shows

- Telegram bot built with `aiogram`
- Browser automation with `Playwright`
- Prompt templates for portrait and style generation
- Queue and lock control for shared browser sessions
- Temporary file handling and cleanup
- Admin controls and lightweight runtime statistics
- Environment-based configuration

## Why It Is Useful

AI image tools are easy to test manually, but harder to turn into a repeatable service. This project focuses on the operational layer around generation:

1. Receive user input in Telegram.
2. Validate and store temporary files.
3. Apply a selected visual preset.
4. Run a controlled browser generation session.
5. Return the result to the user.
6. Keep basic usage and payment statistics.

## Technical Notes

The project uses a local Chrome session controlled by Playwright. This makes it useful as a prototype for teams that want to test visual AI workflows before moving to paid APIs or a dedicated backend service.

For production use, the same logic can be moved behind a provider API, a worker queue, and persistent storage.

## Requirements

- Python 3.10+
- Google Chrome
- Telegram bot token
- Playwright browser dependencies

Install dependencies:

```bash
pip install -r requirements.txt
playwright install chromium
```

Create `.env` from `.env.example`:

```bash
BOT_TOKEN=your_telegram_bot_token
ADMIN_ID=your_telegram_id
PROMO_CODE=2026
ACCOUNTS_POOL=[]
```

Start Chrome with a debug port:

```powershell
"C:\Program Files\Google\Chrome\Application\chrome.exe" --remote-debugging-port=9222 --user-data-dir="C:\chrome_profile"
```

Run the bot:

```bash
python main_pipe.py
```

## Portfolio Notes

This is a proof-of-concept project. The interesting part is not the image model itself, but the automation around it:

- prompt preset system
- browser session control
- user queue handling
- temporary file lifecycle
- Telegram interface for a creative workflow

## Keywords

`python`, `telegram-bot`, `aiogram`, `playwright`, `browser-automation`, `ai-image-generation`, `creative-automation`, `prompt-engineering`, `workflow-automation`

