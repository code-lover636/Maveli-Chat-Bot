# MaveliGPT Chatbot Project

## Introduction

This project is a part of the MaveliGPT competition organized by TinkerHub Toc H Kochi. The aim is to create a chatbot that emulates the wisdom of Maveli.

## Table of Contents

- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Setting up Virtual Environment](#setting-up-virtual-environment)
- [Training the Chatbot](#training-the-chatbot-not-necessary-its-already-trained)
- [Running the Chatbot](#running-the-chatbot)
- [Usage](#usage)
  
## Prerequisites

Before you begin, ensure you have the following installed:

- Python (>=3.6)
- pip

## Installation

1. Clone the repository to your local machine.

```bash
git clone https://github.com/code-lover636/Maveli-Chat-Bot.git
```

2. Navigate to the project directory.

```bash
cd Maveli-Chat-Bot
```

## Setting up Virtual Environment

Create a virtual environment to manage dependencies.

```bash
python3 -m venv venv
```
or 
```
python -m venv venv
```

Activate the virtual environment.

- **Linux/macOS:**

```bash
source venv/bin/activate
```

- **Windows:**

```cmd
venv\Scripts\activate
```
## Installing Rasa
```
pip install rasa
```

## Training the Chatbot (Not necessary; it's already trained)

To train the chatbot model, run the following command:

```bash
rasa train
```

This will use the data in `data/nlu.yml` and `data/stories.yml` to train the chatbot.

## Running the Chatbot

Once the training is complete, you can start the chatbot using the following command:

```bash
rasa run -m models --enable-api --cors "*"
```

The chatbot will be accessible at `http://localhost:5005`.

## Usage

Interact with the chatbot by sending messages through a web-based interface.
