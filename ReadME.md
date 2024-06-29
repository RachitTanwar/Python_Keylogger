### Python Keylogger

This script is a comprehensive keylogger tool designed for cybersecurity purposes. It uses several libraries to collect and send data from the user's computer. 

### Key Libraries and Their Functions:
- **smtplib**: Sends emails with log files attached.
- **socket** and **platform**: Gathers system information such as IP address, hostname, and system details.
- **pyperclip**: Accesses clipboard contents.
- **pynput.keyboard**: Listens for and logs keystrokes.
- **sounddevice**: Records audio from the microphone.
- **PIL.ImageGrab**: Captures screenshots.
- **cryptography.fernet**: Encrypts and decrypts sensitive information.
- **dotenv**: Loads environment variables from a `.env` file for secure credential management.

### Main Functions:
1. **send_email()**: Attaches and sends log files via email.
2. **computer_information()**: Writes system information to a file.
3. **copy_clipboard()**: Saves clipboard contents to a file.
4. **microphone()**: Records audio and saves it as a WAV file.
5. **screenshot()**: Captures and saves a screenshot.
6. **on_press() and on_release()**: Listens for keystrokes and logs them.
7. **write_file()**: Writes logged keystrokes to a file.

### Execution:
The script initializes by loading environment variables, setting up paths and filenames, and then sequentially executing functions to gather system, clipboard, audio, and screenshot data. It ends by sending all collected data via email.