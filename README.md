# DeepSeek-VLM-Chat Webcam Interface

This project integrates the DeepSeek-VL model with a webcam feed and a Gradio web interface. The application captures frames from a live webcam feed and allows users to ask questions about the captured frame using a text-based chat interface. The DeepSeek-VL model processes the frame and provides answers to the questions.

## Features

- **Live Webcam Feed**: Continuously captures frames from the webcam.
- **Frame Capture**: Captures a frame on button press and uses it for inference.
- **Question Answering**: Allows users to ask questions about the captured frame, and the DeepSeek-VL model provides answers.

## Installation

### Prerequisites

- Python 3.7 or later
- CUDA-enabled GPU (for running the model on CUDA)

### Clone the Repository

```bash
git clone https://github.com/deepseek-ai/DeepSeek-VL
cd DeepSeek-VL
```
### Install Dependencies
```bash
pip install gradio opencv-python torch transformers
pip install -e .
```
### Usage
After installing the dependencies mentioned above, 
- run the script [DeepSeek.ipynb](https://github.com/AnshChoudhary/DeepSeek-VLM-Chat/blob/main/DeepSeek.ipynb) on CUDA.
- Open the provided Gradio link to access the web interface. The live webcam feed will be displayed, and you can capture frames and ask questions using the provided buttons and chatbox.
