 1 # E-Tech Agent
    2 
    3 This project is a Python-based agent that uses the Google Agent
      Development Kit (ADK) and the Gemini family of models to provide
      accurate, up-to-date answers to user questions. The agent is equipped
      with a Google Search tool to find the most current and relevant
      information on the web.
    4 
    5 ## Features
    6 
    7 *   **AI-Powered Search:** Leverages a Gemini model to understand user
      queries and process search results.
    8 *   **Real-Time Information:** Integrates directly with Google Search to
      provide answers based on the latest information available.
    9 *   **Asynchronous by Design:** Built with Python's `asyncio` to handle
      operations efficiently without blocking.
   10 *   **Modern Python Packaging:** Uses `pyproject.toml` to manage project
      dependencies and metadata.
   11 
   12 ## Prerequisites
   13 
   14 *   **Python 3.13 or higher.**
   15 *   An active Google Cloud project with the Vertex AI API enabled.
   16 *   Authenticated `gcloud` CLI.
   17 
   18 ## Installation
   19 
   20 This project is managed with modern Python packaging. You can set it up
      using either `uv` (recommended for its speed) or standard `pip`.
   21 
   22 ### 1. Clone the Repository
   23 
   24 First, get the source code by cloning the repository:
  git clone https://github.com/your-username/E-Tech-agent.git
  cd E-Tech-agent

   1 
   2 ### 2. Choose Your Installation Method
   3 
   4 #### Option A: Setup with `uv` (Recommended)
   5 
   6 `uv` is an extremely fast Python package installer and resolver.
   7 
   8 1.  **Install `uv`:**
   9     If you don't have `uv`, you can install it with `pip`:
      pip install uv

   1 
   2 2.  **Create Environment and Install Dependencies:**
   3     `uv` can create a virtual environment and install the project
     dependencies from `pyproject.toml` in a single step.
      uv venv
      uv pip install -e .

   1     *(The `-e .` command installs the project in "editable" mode, which
     is good for development.)*
   2 
   3 3.  **Activate the Environment:**
      source .venv/bin/activate
   1 
   2 #### Option B: Setup with `pip`
   3 
   4 If you prefer to use `pip` and `venv`:
   5 
   6 1.  **Create and Activate a Virtual Environment:**
      python -m venv .venv
      source .venv/bin/activate
   1     *(On Windows, use `.venv\Scripts\activate`)*
   2 
   3 2.  **Install Dependencies:**
   4     `pip` will automatically read the `pyproject.toml` file and install
     the required dependencies.
      pip install -e .

   1 
   2 ## Configuration
   3 
   4 This agent requires access to Google AI services. Before running the
     application, you need to configure your authentication credentials.
   5 
   6 Please follow the official Google Cloud documentation for authenticating.
     For local development, this is typically handled by the `gcloud` CLI:
  gcloud auth application-default login
   1 
   2 ## Usage
   3 
   4 Once your environment is set up and activated, you can run the agent by
     executing the `agent.py` script:
  python agent.py

    1 
    2 The agent will process the default query ("what's the latest ai news?")
      and print the response to the console.
    3 
    4 ## Contributing
    5 
    6 Contributions are welcome! Please feel free to fork the repository, make
      improvements, and submit a pull request.
    7 
    8 ## License
    9 
   10 This project is licensed under the Apache License, Version 2.0.
