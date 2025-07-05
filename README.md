# 🧊 Ice Breaker: Personalized Conversation Starters with AI

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)](https://www.python.org/downloads/)
[![Langchain](https://img.shields.io/badge/Langchain-0.0.354-orange.svg)](https://www.langchain.com/)
[![OpenAI](https://img.shields.io/badge/OpenAI-GPT--3.5-brightgreen.svg)](https://openai.com/)

Tired of generic conversation starters? **Ice Breaker** is an intelligent web application that leverages the power of Large Language Models (LLMs) to generate personalized and engaging icebreakers for any individual. Simply provide a name, and our AI will analyze their professional background to craft unique questions that will spark meaningful conversations.

This project demonstrates a real-world application of the Langchain framework, showcasing how to build powerful LLM-driven tools.

---

## 🚀 About The Project

In today's interconnected world, making a great first impression is more important than ever. Whether you're networking, interviewing, or meeting a new colleague, a well-crafted conversation starter can make all the difference. "Ice Breaker" was built to solve this very problem.

This application uses a sophisticated pipeline to gather information about a person from their LinkedIn profile and then utilizes the creative power of OpenAI's GPT-3.5 to generate insightful and relevant icebreaker questions. It's the perfect tool to help you connect with people on a deeper level.

### Key Features:

* **Personalized Icebreakers:** Generates questions tailored to an individual's career, education, and interests.
* **LinkedIn Integration:** Seamlessly scrapes LinkedIn profiles for up-to-date information.
* **AI-Powered:** Utilizes a `Langchain Agent` with `Chat-GPT 3.5 Turbo` for intelligent and creative question generation.
* **Structured Output:** Employs a `PydanticOutputParser` to ensure the AI's response is always in a clean, usable JSON format.
* **Web Interface:** A user-friendly Flask application to interact with the AI.

---

## 🛠️ Tech Stack

This project is built with a modern, AI-focused technology stack:

* **Framework:** [Langchain](https://www.langchain.com/)
* **LLM:** [OpenAI GPT-3.5 Turbo](https://openai.com/)
* **Web Framework:** [Flask](https://flask.palletsprojects.com/en/3.0.x/)
* **Web Scraping:** [ProxyCurl](https://nubela.co/proxycurl/) & [SerpAPI](https://serpapi.com/)
* **Dependency Management:** [Pipenv](https://pipenv.pypa.io/en/latest/)
* **Testing:** [Pytest](https://docs.pytest.org/en/8.2.x/)

---

## ⚙️ Getting Started

To get a local copy up and running, follow these simple steps.

### Prerequisites

You'll need to have `pipenv` installed on your system. If you don't have it, you can install it with pip:

```bash
pip install pipenv
```

### Installation

Clone the repository:

```bash
git clone https://github.com/emarco177/ice_breaker.git
```

Navigate to the project directory:

```bash
cd ice_breaker
```

Set up your Environment Variables:

Create a `.env` file in the root of the project. Then, copy the contents of `.env.example` into your new `.env` file and add your API keys and project path:

```env
PYTHONPATH=/path/to/your/project/ice_breaker
OPENAI_API_KEY="YOUR_OPENAI_API_KEY"
PROXYCURL_API_KEY="YOUR_PROXYCURL_API_KEY"
SERPAPI_API_KEY="YOUR_SERPAPI_API_KEY"
```

Install Dependencies:

This command will create a virtual environment and install all the required packages from the Pipfile.

```bash
pipenv install
```

### ▶️ Usage

Once the installation is complete, you can start the Flask server to begin generating icebreakers.

Activate the virtual environment and start the Flask server:

```bash
pipenv run python app.py
```

Open your web browser and navigate to `http://127.0.0.1:5000`.

Enter the name of the person you want to research and click "Submit." The application will then process the request and display a set of personalized icebreakers.

### 🧪 Running Tests

To ensure everything is working as expected, you can run the test suite using the following command:

```bash
pipenv run pytest .
```

---
