## Development Purpose Live

For development purposes, you can use `ngrok` to share your local React project with others. Follow these steps:

1. Install `ngrok` globally:

   ```bash
   npm install -g ngrok
   ```

2. Start your React development server:

   ```bash
   npm start
   ```

3. Expose your local server with `ngrok`:

   ```bash
   ngrok http 3000
   ```

   Replace `3000` with your actual port.

   `ngrok` will generate a public URL that you can share for development purposes.

Remember to close the `ngrok` session when you're done sharing.
