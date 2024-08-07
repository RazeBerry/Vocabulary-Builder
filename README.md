# French Vocabulary LaTeX Builder

## Overview

The French Vocabulary LaTeX Builder is a powerful Python-based tool designed to streamline the process of creating and maintaining a comprehensive French vocabulary list in LaTeX format. This application leverages the Anthropic AI API to provide accurate definitions and examples for French words and expressions, making it an invaluable resource for French language learners and educators.

## Features

- **AI-Powered Content Generation**: Utilizes the Anthropic Claude AI to provide definitions and examples for French words.
- **Interactive CLI**: User-friendly command-line interface with rich text formatting.
- **LaTeX Integration**: Automatically generates and inserts LaTeX-formatted entries into your vocabulary document.
- **Alphabetical Sorting**: New entries are inserted in alphabetical order for easy reference.
- **Search Functionality**: Quickly find existing entries in your vocabulary list.
- **Input Validation**: Ensures that entered words meet specific criteria (e.g., length limits).
- **Accent-Insensitive Search**: Allows searching for words with or without accents.

## Prerequisites

- Python 3.6+
- Anthropic API key

## Installation

1. Clone this repository:
   ```
   git clone <repository-url>
   cd french-vocabulary-latex-builder
   ```

2. Install required packages:
   ```
   pip install anthropic rich
   ```

3. Set up your Anthropic API key:
   - Create a `.env` file in the project root.
   - Add your API key: `ANTHROPIC_API_KEY=your_api_key_here`

## Usage

1. Run the script:
   ```
   python french_vocab_builder.py
   ```

2. Follow the on-screen prompts to:
   - Add new French words or expressions
   - Search existing entries
   - Exit the application

3. The script will update your LaTeX file (`FrenchVocab.tex`) with new entries automatically.

## Configuration

- Modify the `latex_file` variable in `main()` to point to your LaTeX file location.
- Adjust the `max_word_length` in the `FrenchVocabBuilder` class to change the maximum allowed word length.

## LaTeX Structure

The script generates LaTeX entries in the following format:

```latex
\entry{Word}{Type}
{
    \item Definition 1
    \item Definition 2
}
{
    \item French example 1 \\ (English translation 1)
    \item French example 2 \\ (English translation 2)
}
```

Ensure your LaTeX document is set up to handle this structure.

## Contributing

This is a personal project, but suggestions for improvements are welcome. Feel free to fork the repository and submit pull requests.

## License

This project is for personal use and does not have a specific license attached to it.

## Acknowledgments

- Anthropic for providing the Claude AI API
- Rich library for enhancing the CLI experience

---

Happy French learning!
