E-Tech Agent
E-Tech Agent is a Python-based intelligent agent built with the Google Agent Development Kit (ADK) and the Gemini model family. It provides high-quality, real-time answers by integrating directly with Google Search and processing results using advanced language capabilities.

Features

AI-Enhanced Search: Uses a Gemini model to interpret user intent and synthesize high-value answers from search results.

Real-Time Information Retrieval: Connects to Google Search to deliver the most current and relevant insights.

Async Architecture: Built using asyncio to maximize efficiency and non-blocking operations.

Modern Packaging: Managed through pyproject.toml for clean, modern dependency and build management.

Prerequisites

Python 3.13+

A Google Cloud project with Vertex AI API enabled

Authenticated gcloud CLI session

Installation

You can install the project using either uv (recommended) or pip.

1. Clone the Repository
git clone https://github.com/your-username/E-Tech-agent.git
cd E-Tech-agent

2. Installation Methods
Option A: Using uv (Recommended)

uv provides faster installation and dependency resolution.

1. Install uv
pip install uv

2. Create the Environment and Install Dependencies
uv venv
uv pip install -e .


(Installing with -e . places the project in editable mode for active development.)

3. Activate the Environment
source .venv/bin/activate

Option B: Using pip
1. Create and Activate a Virtual Environment
python -m venv .venv
source .venv/bin/activate


(Windows: .venv\Scripts\activate)

2. Install Dependencies
pip install -e .

Configuration

Authentication is required to access Google AI services. Ensure your Google Cloud credentials are properly configured.

Run:

gcloud auth application-default login

Usage

Once installed and configured, run the agent:

python agent.py


The agent will execute with a default query—"what's the latest AI news?"—and display the processed response.

Contributing

Contributions are encouraged. Fork the repository, implement improvements, and submit a pull request.

License

This project is available under the Apache License 2.0.