# FlightAI Chat Assistant

This project implements a conversational AI assistant for an airline, FlightAI, using OpenAI's GPT models and Gradio for the user interface. The assistant provides concise, accurate answers and supports tool integration for ticket pricing, image generation, and text-to-speech audio responses.

---

## Features

- Chatbot powered by `gpt-4o-mini` model with a system prompt to keep replies short and courteous.
- Tool integration to fetch ticket prices for specific cities.
- Image generation using DALL-E 3 to create city-related vacation images.
- Text-to-speech audio responses using OpenAI's speech model.
- Interactive Gradio interface combining chat, images, and audio playback.

---

## Setup

1. Install dependencies:
   ```bash
   pip install openai gradio python-dotenv pillow pydub
   ```
2. Create a .env file with your OpenAI API key:
   ```bash
   OPENAI_API_KEY=your_api_key_here
   ```
3. Run the script.

## Code Overview
- Environment and API Initialization: Loads environment variables, initializes OpenAI client.
- System Message: Defines the assistant’s behavior and tone.
- Ticket Pricing Tool: Provides ticket prices for select cities.
- Image Generation: Generates pop-art style vacation images for requested cities.
- Audio Generation: Converts assistant's text replies to speech and plays them.
- Chat Function: Handles conversation flow, tool calls, and multi-modal outputs.
- Gradio UI: Custom chat interface with message input, chat history, image display, and clear button.

## Usage
- Launch the Gradio interface.
- Chat naturally with the assistant.
- Ask about ticket prices or request vacation images.
- Hear replies read aloud automatically.

## Notes
- The API key must be set for the script to work.
- FFmpeg is required for audio playback (pydub dependency).
- Image and audio generation require internet access and valid API credentials.

