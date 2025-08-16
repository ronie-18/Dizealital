# Dizealital Contact Form Backend

## Setup

1. Install dependencies (already done):
   ```bash
   npm install
   ```

2. Create a `.env` file in the backend directory with the following content:
   ```env
   GMAIL_USER=dizealital@gmail.com
   GMAIL_PASS=YOUR_GMAIL_APP_PASSWORD_HERE
   ```
   - For Gmail, you must use an App Password (not your regular Gmail password). See: https://support.google.com/accounts/answer/185833

3. Start the server:
   ```bash
   node index.js
   ```

## API Endpoint
- **POST** `/contact`
- **Body:** JSON `{ name, email, message }`
- **Response:** `{ success: true, message: 'Message sent successfully!' }` or error
