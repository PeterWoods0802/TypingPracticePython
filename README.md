Below is an example of a visually appealing and informative GitHub README file for your project:

---

```markdown
# Typing Practice Program

A simple Python-based typing practice program built with Tkinter that helps you improve your typing skills. Choose between using an English dictionary (loaded from a file) or your own custom words, and challenge yourself with timed rounds of 20 random words!

## Features

- **Configurable Word Source:**  
  Choose between using an English dictionary loaded from a file (`dictionary.txt`) or entering your own custom words.
  
- **Timed Rounds:**  
  A timer starts with your first keystroke and records the time it takes to complete each round of 20 words.
  
- **Real-Time Visual Feedback:**  
  The program underlines the next character to type in red. Only correct keystrokes advance the underline.
  
- **Simple & Clean Interface:**  
  Built with Tkinter for an easy-to-use graphical interface.

## Getting Started

### Prerequisites

- **Python 3.x**  
  Tkinter comes pre-installed with Python, so no additional packages are required.

### Installation

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/yourusername/typing-practice.git
   cd typing-practice
   ```

2. **(Optional) Create a Virtual Environment:**

   ```bash
   python -m venv venv
   source venv/bin/activate    # On Windows: venv\Scripts\activate
   ```

### Dictionary Setup

Create a file named `dictionary.txt` in the project directory and add your list of words. Words can be separated by spaces or placed on separate lines. This file will be used when you select the "English Dictionary" option.

### Running the Program

Run the script using:

```bash
python typing_practice.py
```

## How It Works

1. **Configuration Screen:**  
   On launch, a window appears allowing you to choose:
   - **English Dictionary:** Uses words from `dictionary.txt`.
   - **Custom:** Lets you enter your own words (separated by spaces).

2. **Typing Test:**  
   After clicking **Start**, 20 random words are displayed with the next character to type underlined in red. The timer begins on your first key press.
   
3. **Real-Time Feedback:**  
   - **Correct Keystroke:** The underline moves to the next character.
   - **Incorrect Keystroke:** No progress is made until the correct key is pressed.

4. **Round Completion:**  
   When you finish typing the 20 words, the elapsed time is shown as "Last time" at the top. The timer resets for each new round.

## Code Overview

### Main Components

- **Configuration Frame:**  
  Presents options for selecting the word source and entering custom words.

- **Test Frame:**  
  Displays the 20-word challenge, current round timer, and the last round's elapsed time.

- **Typing Logic:**  
  Captures keystrokes, compares them with the expected character, and updates the display accordingly.

- **Timer Functionality:**  
  Initiates on the first keystroke, updates continuously, and stops when the round is complete.

### Key Functions

- **`load_dictionary(filename)`**  
  Loads words from `dictionary.txt`. If the file is missing, a fallback list is used.

- **`start_test()`**  
  Processes the selected word source and transitions from the configuration screen to the test screen.

- **`new_round()`**  
  Generates a new round with 20 random words and resets the timer.

- **`update_text_display()`**  
  Renders the text for the current round and underlines the next character to be typed.

- **`handle_keypress(event)`**  
  Validates keystrokes, advances the underline on correct entries, and manages round completion.

- **`update_timer()`**  
  Refreshes the timer display at regular intervals while the round is in progress.

## Contributing

Contributions, issues, and feature requests are welcome! Please feel free to check the [issues page](https://github.com/yourusername/typing-practice/issues) or submit a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

## Acknowledgements

- Built using Python's Tkinter library.
- Inspired by various online typing practice programs and educational tools.

---

Enjoy improving your typing speed and accuracy!
```

---

Simply copy this text into a `README.md` file in your repository, adjust the repository URL and any other details as needed, and you'll have an informative and visually appealing README page for your project!
