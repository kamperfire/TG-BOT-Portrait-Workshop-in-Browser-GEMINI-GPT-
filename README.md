# 📸 Portrait Workshop

A professional tool for creating photorealistic portraits and artistic stylizations based on the advanced image creation models of Gemini and ChatGPT.
Everything can be edited and customized to your needs, the project was created in January 2026, and it has not been further developed. As an alternative, you can convert it to an API structure, which will make it simpler and faster, but you will need to pay for the API.
---

## 🌟 About the project

**Auto-Creative-Pipe** is not just a bot, it is a full-fledged "conveyor" of creativity. It takes your regular selfie (the better the photo quality, the better) and, preserving your facial features with 100% accuracy, transports you to luxurious interiors, magazine covers, or fairy-tale worlds.

### What this bot can do:
*   **💎 Wealth and Luxury Mode:** Find yourself on a private jet, a yacht in Amalfi, or in the office of a top manager.
*   **🎬 Cinematic Noir:** Dramatic lighting, smoke, deep shadows, and a Hollywood movie atmosphere.
*   **🎄 Holiday Magic:** New Year's decorations, cozy winter evenings, and fairy-tale transformations.
*   **👫 Couple and Group Photos:** Create joint portraits with friends or your significant other in a unified style.
*   **🎨 Your Own Style:** Just describe in words what you want to see, and the AI will bring it to life.

---

## 🚀 How it works (Technical part)

The bot is built on a unique combination of technologies that provide the highest quality without using paid APIs (emulating user actions):

1.  **Playwright Automation:** The bot controls a real Chrome browser, simulating human behavior in the Gemini and ChatGPT interfaces. This allows you to bypass API limitations and access the most powerful generation models using only a Pro or Go subscription.
2.  **Face Consistency (Preservation of the face):** Specially designed prompts and image submission algorithms force the neural network to use the original photo as a hard reference, preserving facial expressions and features.
3.  **Hybrid generation:**
    *   **Standard (Gemini):** Lightning speed, high clarity and realism.
    *   **Premium (chatGPT):** Artistic depth, working with composition and complex requests.

---

## 🛠 Installation and launch

### 1. Requirements
*   Python 3.10+
*   Google Chrome (with remote control capability)
*   Installed dependencies: `pip install -r requirements.txt`

### 2. Setting up the environment (`.env`)
Create a `.env` file in the root folder:
```env
BOT_TOKEN=your_telegram_bot_token
ADMIN_ID=your_telegram_id
PROMO_CODE=2026
ACCOUNTS_POOL=["email1@gmail.com ", "email2@gmail.com "] # For ChatGPT rotation, different browsers may work differently
``

###3. Launching the browser
For the bot to work, you need to run Chrome with the debug port open (9222). 
**For Windows ('run_chrome.bat'):**
``batch
"C:\Program Files\Google\Chrome\Application\chrome.exe" --remote-debugging-port=9222 --user-data-dir="C:\chrome_profile"
```

### 4. Starting the bot
```bash
python main_pipe.py
```

---

## 📊 Control Panel (Dashboard)
The bot is equipped with an advanced real-time console dashboard:
* **Uptime and Queue:** Monitor the load on the VPS.
* **Log of actions:** See every request, every payment, and the generation status.
*   **Finance:** Automatically calculate your daily, weekly, and monthly income.

---

## 🛡 Security and Stability
*   **Database (JSON):** Lightweight and fast user management.
*   **Lock System:** Prevents conflicts when multiple users use the browser simultaneously.
*   **Auto-Cleaning:** Temporary files are automatically deleted after submission.

---
**This project has been tested by a base of 1000 people, in principle, from the problems I can note children's censorship in chatGPT, in Gemini such problems are at times less. By downloading 1 account of Gemini, it is enough for 50 generations in 2 hours, chatGPT for 20 generations per hour~

*Designed with love for detail.❤️ *