# PythonAgentAI

This project leverages various query engines and an agent to provide detailed information about world demographics and specific details about India. It utilizes a combination of Python libraries and OpenAI's GPT-3.5 model to process and respond to queries.

## Features

- Query world population and demographics data.
- Access detailed information about India from a custom PDF engine.
- Utilize a ReActAgent to handle and respond to user prompts.
- Load environment variables using `dotenv`.

## Prerequisites

Before running the project, ensure you have the following installed:

- Python 3.8 or higher
- Required Python libraries (listed in `requirements.txt`)

## Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/srishti2207/Python_Agent_AI.git
    cd Python_Agent_AI
    ```

2. Create a virtual environment and activate it:

    ```bash
    python3 -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. Install the required packages:

    ```bash
    pip install -r requirements.txt
    ```

4. Set up environment variables:

    Create a `.env` file in the root directory and add your environment variables. Example:

    ```plaintext
    OPENAI_API_KEY=your_openai_api_key
    ```

5. Ensure the data file `population.csv` is placed in the `data` directory.

## Usage

1. Run the main script:

    ```bash
    python main.py
    ```

2. Enter prompts to query the data. To quit, type `q`.

## Project Structure

- `main.py`: Main script to run the query engine and agent.
- `prompts.py`: Contains prompt templates and instructions.
- `note_engine.py`: Defines the note engine used as a tool by the agent.
- `pdf.py`: Contains the India PDF engine for querying detailed information about India.
- `data/population.csv`: CSV file containing world population and demographics data.

## Customization

- To update the population query prompts, modify the `new_prompt` and `instruction_str` in `prompts.py`.
- To change the data sources, update the paths and files in `main.py`.

