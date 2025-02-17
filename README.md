# Mathswatch Autosolver

## Description
This userscript automates the process of solving questions on the Mathswatch platform. It captures an image of a question from the Mathswatch website, sends it to Gemini (a Google AI model), and displays the answer in a beautifully styled new tab.

## Features
- Captures images from questions with the class `img-responsive col-xs-12 img-question` on the Mathswatch website.
- Sends the image to the Gemini API for analysis.
- Displays the generated answer in a new tab with a user-friendly, modern interface.
- Allows users to copy the generated answer to their clipboard.
  
## Installation

### 1. Install a Userscript Manager
To use this script, you'll need to install a userscript manager, such as:
- [Tampermonkey](https://www.tampermonkey.net/) (recommended)
- [Greasemonkey](https://www.greasespot.net/)

### 2. Add the Script
1. Open your userscript manager (Tampermonkey/Greasemonkey).
2. Create a new script and paste the entire code from the `Mathswatch Autosolver` script above.
3. Save the script.

### 3. Get API Key
- You'll need a Google AI Studio API key to use this script. You can get one from [Google AI Studio](https://cloud.google.com/ai).
- Once you have your API key, paste it into the script at the line: `const GEMINI_API_KEY_KEY = 'Your-Google-API-Key-Here';`.

### 4. Use the Script
- After installation, visit the Mathswatch website (`https://vle.mathswatch.co.uk`).
- Press `Ctrl + X` on your keyboard to trigger the script. The script will capture an image of the current question and send it to Gemini for analysis.
- Once the answer is returned, it will be displayed in a new tab, where you can copy it to your clipboard.

## Configuration
You can customize the default prompt sent to Gemini by editing the `DEFAULT_PROMPT` variable. The current default is:

