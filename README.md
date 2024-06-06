# GitHub Issues Assistant

The GitHub Issues Assistant is a powerful tool that enables users to ask questions about GitHub issues and receive informative responses. It leverages various libraries and technologies to fetch and process GitHub issues data, store it in a vector database, and generate responses using a state-of-the-art language model.

## Features

- Fetches GitHub issues data from a specified repository using the GitHub API
- Stores the fetched issues in an AstraDB vector database for efficient retrieval
- Utilizes OpenAI's language model to generate informative responses to user queries
- Provides a user-friendly web interface using Gradio for easy interaction

## Installation

1. Clone the repository:

   ```
   git clone https://github.com/Akshat2634/GitHub-Agent
   ```

2. Install the required dependencies:

   ```
   pip install -r requirements.txt
   ```

3. Set up the environment variables in a `.env` file:
   ```
   GITHUB_TOKEN=your-github-token
   ASTRA_DB_API_ENDPOINT=your-astradb-api-endpoint
   ASTRA_DB_APPLICATION_TOKEN=your-astradb-application-token
   ASTRA_DB_KEYSPACE=your-desired-keyspace
   ```

## Usage

1. Run the main script:

   ```
   python main.py
   ```

2. Access the web interface by opening the provided URL in your web browser.

3. Enter your question about GitHub issues in the input field and click "Submit" to receive a response.

## Libraries Used

The GitHub Issues Assistant utilizes the following libraries:

- [requests](https://docs.python-requests.org/): A simple, yet elegant, HTTP library for making API requests.
- [python-dotenv](https://github.com/theskumar/python-dotenv): Reads key-value pairs from a `.env` file and sets them as environment variables.
- [langchain](https://github.com/hwchase17/langchain): A framework for developing applications powered by language models.
- [OpenAI](https://openai.com/): Provides access to OpenAI's powerful language models.
- [Gradio](https://gradio.app/): A Python library for building web interfaces for machine learning models.
- [AstraDB](https://www.datastax.com/products/datastax-astra): A scalable and fast vector database for efficient data retrieval.

## Project Structure

```
.
├── main.py
├── github.py
├── note.py
├── .env
├── requirements.txt
├── LICENSE
└── README.md
```

- `main.py`: The main script that sets up the GitHub Issues Assistant and launches the web interface.
- `github.py`: Contains functions for fetching GitHub issues data using the GitHub API.
- `note.py`: Defines a custom tool for taking notes during the question-answering process.
- `.env`: Environment file to store sensitive information like API tokens and endpoints.
- `requirements.txt`: Lists the required Python dependencies.
- `LICENSE`: The license file for the project.
- `README.md`: This readme file providing an overview of the project.

## Contributing

Contributions are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request.

## License

This project is licensed under the [MIT License](LICENSE).

## Acknowledgements

- [Langchain](https://github.com/hwchase17/langchain) for providing the language model and agent functionality.
- [OpenAI](https://openai.com/) for the powerful language model used in this project.
- [AstraDB](https://www.datastax.com/products/datastax-astra) for the scalable and fast vector database.
- [Gradio](https://gradio.app/) for the user-friendly web interface.
