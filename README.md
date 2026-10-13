# Run and Deploy Your AI Studio App

This repository contains the code needed to run your AI Studio app locally.

**Open the app in Google AI Studio:**  
https://ai.studio/apps/bdbe5719-0d85-4a20-a223-790818a3bc7e

## Prerequisites

- [Node.js](https://nodejs.org/) installed
- npm installed
- A valid Gemini API key

## Run Locally

1. Clone or download this repository.
2. Open a terminal in the project directory.
3. Install the dependencies:

   ```bash
   npm install
   ```

4. Create a local `.env.local` file in the project root and configure your Gemini API key using the environment variable expected by the application:

   ```env
   GEMINI_API_KEY=your_api_key_here
   ```

5. Start the development server:

   ```bash
   npm run dev
   ```

6. Open the local URL displayed in the terminal.

## Security Notes

- Never commit your real API key to GitHub.
- Keep `.env.local` out of version control.
- Use `.env.example` to document required environment variable names without including secrets.
- If an API key is accidentally exposed, revoke it and generate a replacement.

## Troubleshooting

- If `npm install` fails, check your Node.js and npm versions.
- If the app cannot access Gemini, verify that the API key is valid and that the environment variable name matches the application code.
- If the development server fails to start, review the terminal error messages.
