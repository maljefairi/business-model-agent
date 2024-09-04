# Business Model Generator with Ollama Gemma2

This project is a Business Model Generator that uses the Ollama Gemma2 language model to create comprehensive business models based on a project title and description.

## Features

- Generates a detailed business model with 10 key sections
- Uses the Ollama Gemma2 model for high-quality, context-aware content generation
- Outputs the business model as a formatted Microsoft Word document

## Prerequisites

Before you begin, ensure you have met the following requirements:

- Python 3.7 or higher
- Ollama installed with the Gemma2 model (see installation instructions below)

## Installation

1. Clone this repository:
   ```
   git clone https://github.com/yourusername/business-model-generator.git
   cd business-model-generator
   ```

2. Create and activate a virtual environment:
   ```
   python -m venv .venv
   source .venv/bin/activate  # On Windows, use `.venv\Scripts\activate`
   ```

3. Install the required Python packages:
   ```
   pip install -r requirements.txt
   ```

4. Install Ollama:
   Follow the instructions at [Ollama's official website](https://ollama.ai/download) to install Ollama for your operating system.

5. Install the Gemma2 model:
   After installing Ollama, run the following command:
   ```
   ollama pull gemma2
   ```

## Usage

1. Ensure the Ollama service is running.

2. Modify the `project_title` and `project_description` variables in the `main()` function of `bmOllama.py` to match your project.

3. Run the script:
   ```
   python bmOllama.py
   ```

4. The generated business model will be saved as a Word document in the same directory as the script.

## Project Structure

- `bmOllama.py`: Main script containing the business model generation logic
- `requirements.txt`: List of Python dependencies
- `.gitignore`: Specifies intentionally untracked files to ignore

## Dependencies

This project relies on the following Python packages:

- certifi==2024.8.30
- charset-normalizer==3.3.2
- idna==3.8
- lxml==5.3.0
- python-docx==1.1.2
- requests==2.32.3
- typing_extensions==4.12.2
- urllib3==2.2.2

## Notes

- The generated Word document (`.docx` file) is ignored by Git as specified in the `.gitignore` file.
- Make sure to keep your virtual environment (`.venv`) directory excluded from version control.

## Contributing

Contributions to this project are welcome. Please fork the repository and submit a pull request with your changes.

## License

This project is licensed under the MIT License - see the LICENSE file for details.
