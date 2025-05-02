# Telegram File Uploader Bot

A Flask-based Telegram bot for uploading files to a channel and managing them, deployed on Vercel.

## Features
- Upload documents, photos, videos, and audio files to a Telegram channel.
- Get shareable links for uploaded files.
- Delete files using a button.
- Admin commands for managing files and users.
- Privacy policy page.

## Project Structure
```
project/
├── api/
│   └── index.py          # Main Flask application
├── templates/            # HTML templates (optional, embedded in index.py)
├── .gitignore
├── LICENSE
├── README.md
├── requirements.txt
├── vercel.json
```

## Setup
1. **Clone the Repository**:
   ```bash
   git clone <repository-url>
   cd <repository-name>
   ```

2. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

3. **Set Up Environment Variables**:
   Create a `.env` file with the following:
   ```
   TELEGRAM_TOKEN=your-telegram-bot-token
   CHANNEL_USERNAME=@yourchannel
   ADMIN_IDS=your-admin-id
   MAX_FILE_SIZE_MB=4000
   RATE_LIMIT=Infinity
   BOT_USERNAME=your-bot-username
   KV_URL=your-vercel-kv-url
   KV_REST_API_URL=your-vercel-kv-rest-api-url
   KV_REST_API_TOKEN=your-vercel-kv-rest-api-token
   KV_REST_API_READ_ONLY_TOKEN=your-vercel-kv-rest-api-read-only-token
   ```

4. **Deploy to Vercel**:
   - Push the code to a Git repository.
   - Connect the repository to Vercel and deploy.
   - Set the environment variables in Vercel's dashboard.

5. **Set Webhook**:
   After deployment, visit `https://your-app.vercel.app/setwebhook` to set the Telegram webhook.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
