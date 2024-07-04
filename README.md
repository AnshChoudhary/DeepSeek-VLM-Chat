# DeepSeek-VLM-Chat Webcam Interface

This project integrates the DeepSeek-VL model with a webcam feed and a Gradio web interface. The application captures frames from a live webcam feed and allows users to ask questions about the captured frame using a text-based chat interface. The DeepSeek-VL model processes the frame and provides answers to the questions.

## DeepSeek-VL 
DeepSeek-VL is an open-source vision-language model designed for real-world applications that require understanding both visual and textual information. It combines capabilities in image and text processing to perform a variety of tasks, such as logical diagram analysis, webpage understanding, formula recognition, and interaction with scientific literature and natural images.

The model uses a hybrid vision encoder that supports high-resolution image input (up to 1024x1024 pixels) and is built on the DeepSeek-LLM-7b-base, trained on approximately 2 trillion text tokens. The training process for DeepSeek-VL involves around 400 billion vision-language tokens, ensuring a comprehensive understanding of both modalities. This extensive training enables the model to excel in tasks such as optical character recognition (OCR), visual question answering, and chatbot functionalities.

DeepSeek-VL is structured to handle a wide range of real-world scenarios and datasets, making it particularly versatile for practical applications. It achieves competitive performance across various benchmarks while maintaining efficient computational requirements​.

![Sample Responses](https://github.com/AnshChoudhary/DeepSeek-VLM-Chat/blob/main/sample-deepseek.jpg)

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
