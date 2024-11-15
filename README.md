
# Google-Meet-Bot

This project is a Python bot that automates the process of logging into Gmail, joining a Google Meet, recording the audio of the meeting, and then generating a summary, key points, action items, and sentiment analysis of the meeting.

## Prerequisites

- Python 3.8 or higher
- Chrome browser
- OpenAI API Key
- A Gmail account
- A Google Meet link
- FFmpeg (included in the repo as a `.zip` file)

## Installation

1. Clone the repository:

   ```bash
   git clone <repository-url>
   cd google-meet-bot
   ```

2. Set up the Python environment:

   ```bash
   python -m venv env
   ```

3. Activate the environment:
   - For Ubuntu:
     ```bash
     source env/bin/activate
     ```
   - For Windows:
     ```bash
     env\scripts\activate
     ```

4. Install the required dependencies:

   ```bash
   pip install -r requirements.txt
   ```

5. Set Up FFmpeg:
   - The repository includes an FFmpeg `.zip` file.
   - Unzip the file to a directory (e.g., `C:\ffmpeg` on Windows).
   - Add the FFmpeg `bin` directory to your system’s environment variables to use it globally.

### Adding FFmpeg to the System Path (Windows)

1. Open Command Prompt as Administrator.
2. Use the following command to add the FFmpeg path:
   ```cmd
   setx PATH "%PATH%;C:\ffmpeg\bin" /M
   ```
3. Close and reopen Command Prompt to refresh the environment. You can verify the installation by running:
   ```cmd
   ffmpeg -version
   ```

6. Run the Script:

   ```bash
   python join_google_meet.py
   ```
