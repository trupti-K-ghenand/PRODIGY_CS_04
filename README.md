#PRODIGY_CS_04
# 🖥️ Simple Keylogger
Internship Task_04 at Prodigy InfoTech

## 📜 Overview
This program implements a basic keylogger using Python. The keylogger captures and logs keystrokes, providing options to start logging, stop logging, and save the log to a file. 
**Note:** Ethical considerations and permissions are crucial for projects involving keyloggers.

## 📚 Theoretical Explanation

### 🔐 Keylogging
Keylogging is the action of recording the keys struck on a keyboard, typically in a covert manner, 
so that the person using the keyboard is unaware that their actions are being monitored. 
Keyloggers can be used for legitimate purposes like monitoring employee activity or for malicious purposes like stealing personal information.

### 🛡️ Cybersecurity Concepts
- **Ethical Use:** Keyloggers should only be used with proper authorization and for legitimate purposes.
- **Privacy Concerns:** Unauthorized keylogging can lead to significant privacy violations and is illegal in many jurisdictions.
- **Data Security:** Ensure that the logged data is securely stored and accessed only by authorized individuals.

## 📝 Prerequisites
- Basic understanding of Python programming.
- Familiarity with GUI development using Tkinter.
- Knowledge of threading and handling keyboard events.

## 💻 Software Requirements
- Python 3.x
- Libraries: `pynput`, `tkinter`

## 🖥️ Hardware Requirements
- A computer with at least 2GB of RAM.
- Any operating system that supports Python 3.x.

## 🛠️ Tech Stack
- **Programming Language:** Python
- **Libraries:** Tkinter, Pynput, Threading

## 🚀 How to Execute the Program

1. **Clone the Repository:**
   ```bash
   git clone <repository-directory> (https://github.com/trupti-K-ghenand/PRODIGY_CS_04)
   cd <repository-directory>
   ```

2. **Install the Required Libraries:**
   ```bash
   pip install pynput
   ```

3. **Run the Program:**
   ```bash
   python task4_keylogger.py
   ```

4. **Usage Instructions:**
   - Click on "Start Logging" to begin capturing keystrokes.
   - Click on "Stop Logging" to stop capturing keystrokes.
   - Click on "Save Log" to save the captured keystrokes to a text file.

## 📄 Code Details Overview

### `task4_keylogger.py`

#### Imports
```python
import tkinter as tk
from tkinter import filedialog, messagebox
from pynput import keyboard
import threading
```
- `tkinter`: For creating the GUI application.
- `pynput`: For capturing keyboard inputs.
- `threading`: For handling concurrent execution of keylogging and GUI operations.

#### `Keylogger` Class
- **Attributes:**
  - `log`: Stores the captured keystrokes.
  - `is_logging`: Boolean flag to check if logging is active.
  - `listener`: Keyboard listener object.
- **Methods:**
  - `__init__(self, root)`: Initializes the GUI components.
  - `start_logging(self)`: Starts the keylogging process.
  - `stop_logging(self)`: Stops the keylogging process.
  - `on_press(self, key)`: Captures and logs each key press.
  - `save_log(self)`: Saves the captured keystrokes to a file.

#### GUI Setup
- **Main Window**: The root window is set up with a title and dimensions.
- **Label**: Displays instructions to the user.
- **Buttons**: Start, Stop, and Save Log buttons to control the keylogging process.

#### Running the Application
```python
if __name__ == "__main__":
    root = tk.Tk()
    app = Keylogger(root)
    root.mainloop()
```
- The application initializes the `Keylogger` class and starts the Tkinter main loop.

## ⚠️ Ethical Considerations
- Always inform users that their keystrokes are being logged.
- Obtain explicit permission from users before deploying a keylogger.
- Use keyloggers for ethical and legitimate purposes only.
- 
## Thanks👏
Thank you for using and contributing to this repository! I sincerely appreciate your interest and hope you find the keylogger program helpful for your Cyber Security learning journey.

## Contribute🤝
Welcome all contributions to enhance these programs and expand their capabilities.

To contribute:
1. Fork the repository.
2. Create a new branch for your feature or bugfix.
3. Commit your changes and push them to your branch.
4. Open a pull request describing your changes.

✅Please ensure your code adheres to the existing style and includes appropriate documentation and tests.


## 🛡️Secure coding!🛡️


