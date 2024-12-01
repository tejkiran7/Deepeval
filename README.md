# Deepeval
DeepEval is an open-source evaluation framework for LLMs. DeepEval makes it extremely easy to build and iterate on LLM (applications) and was built with the following principles in mind:

Easily "unit test" LLM outputs in a similar way to Pytest.<br>
Plug-and-use 14+ LLM-evaluated metrics, most with research backing.<br>
Synthetic dataset generation with state-of-the-art evolution techniques.<br>
Metrics are simple to customize and covers all use cases.<br>
Real-time evaluations in production.

## Prerequisites

- Python 3.7 or higher
- Required Python packages listed in `requirements.txt`

## Installation

1. Clone the repository:
   ```bash
   git clone <repository_url>
   cd <repository_name>

2. Install the required dependencies:
    ```bash
    pip install -r requirements.txt

## Setup

1. Create an .env file in the project root directory and add the following keys:
  ```bash
  OPENAI_API_KEY=<your_openai_api_key>
  GOOGLE_API_KEY=<your_google_api_key>
  ```
Replace <your_openai_api_key> and <your_google_api_key> with your actual API keys.

## Running the Script
If you are running text_example.py, you must set the OPENAI_API_KEY in your terminal. Ensure the .env file is correctly configured as described above.

1.  Set the OPENAI_API_KEY in the terminal:
   ```bash
  set OPENAI_API_KEY=<your_openai_api_key> # Windows
  export OPENAI_API_KEY=<your_openai_api_key> # macOS/Linux
  ```

2.  Run the script:
  ```bash
   deepeval test run test_example.py
```

## Notes
Ensure your .env file is not committed to your repository by adding it to .gitignore. Add the following line to .gitignore:
```bash
.env
```
