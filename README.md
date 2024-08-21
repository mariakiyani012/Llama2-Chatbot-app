# Llama 2 Chatbot

This project is a simple web-based chatbot application built using Streamlit and powered by the Llama 2 model via the Replicate API. The chatbot allows users to interact with the Llama 2 model, generating responses based on user input.

## Features

- **Select Llama 2 Model:** Choose between different Llama 2 models (7B, 13B, 70B) for generating responses.
- **Customize Parameters:** Adjust temperature, top_p, and max_length for fine-tuning the responses.
- **Interactive Chat Interface:** Engage in a chat-like interface with stored message history.
- **Clear Chat History:** Option to clear chat history to start fresh.

## Getting Started

### Prerequisites

- Python 3.8 or higher
- Streamlit
- Replicate API token


### Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/mariakiyani012/llama2-chatbot.git
   cd llama2-chatbot

2. **Install the required Python packages:**

   ```bash
   pip install -r requirements.txt
   ```

### Configuration

1. **Add your Replicate API token:**

   To use the Replicate API, you need to provide your API token. Create a `.streamlit/secrets.toml` file in the root of your project and add the following:

   ```toml
   [general]
   REPLICATE_API_TOKEN = "your_replicate_api_token_here"
   ```

   Alternatively, you can enter your API token directly in the app when prompted.

### Running the App

1. **Run the Streamlit app:**

   ```bash
   streamlit run app.py
   ```

   If you've named the main script differently, replace `app.py` with your script's name.

2. **Open the app in your browser:**

   The app will automatically open in your default web browser. If not, go to `http://localhost:8501` to access the Llama 2 Chatbot.

### Usage

1. **Select a Llama 2 Model:**

   From the sidebar, choose between Llama2-7B, Llama2-13B, and Llama2-70B models based on your requirements.

2. **Adjust Parameters:**

   Use the sliders in the sidebar to adjust `temperature`, `top_p`, and `max_length` to control the behavior of the generated responses.

3. **Chat with the Bot:**

   Enter your message in the input box at the bottom and press Enter. The chatbot will generate a response using the selected Llama 2 model.

4. **Clear Chat History:**

   Use the "Clear Chat History" button in the sidebar to reset the conversation.

### Project Structure

```
├── app.py                 # Main Streamlit app
├── requirements.txt       # Python dependencies
├── .streamlit/
│   └── secrets.toml       # Replicate API token configuration (Not included in the repo)
└── README.md              # Project documentation
```

### License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
