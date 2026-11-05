# Vision Analytics Demo on HPE Private Cloud AI

This project demonstrates a powerful, interactive application to analyse images, videos, and real-time video streams using a Vision Language Model (VLM). The application is built with Gradio, containerized with Docker, and designed for seamless deployment on **HPE Private Cloud AI (PCAI)** using a reusable Helm chart.

Users can analyse an image, video clip, or connect a live rtsp stream with a  deployed VLM with a custom prompt to extract structured information.


---

### Context on Customer and Use Case

This demo is ideal for customers looking to analyse images, video, or live streams to automate manual visual inspection.

### Solution Overview and Demo Video

- [Solution Overview]
- [Demo Video]

---

### Key Features
*   **VLM Configuration:** Configure the VLM's API endpoint and key directly within the Gradio UI, allowing for easy switching between different models or environments.
*   **Image Analysis Tab :** Upload an image and enter prompt to extract visual insights from image.
*   **Video Understanding Tab :** Upload an video and enter prompt to extract visual insights from image. Vision understanding is configure to select number of frame, framerate, and the amount of duration to analyse
*   **On-Demand Live RTSP Steam Analysis:** Capture a single frame from any live stream and send it to a Vision Language Model for analysis.
*   **Structured Data Extraction:** The VLM prompt in RSTP Stream Tab, its configurable to return structured data (e.g., vehicle type, colour, status), which the application parses into a clean JSON object.
*   **Data Export:** Download the parsed JSON data for any analysis with a single click.
*   **HPE PCAI Optimized:** Packaged as a Helm chart that integrates with PCAI's Istio gateway and "Tools & Frameworks" deployment model.

---

## Prerequisites

### 1. Model Deployment in HPE PCAI

This application requires a Vision Language Model to be deployed and running within the HPE Machine Learning Inference Software Tool.

*   **Model:** `Qwen/Qwen2.5-VL-32B-Instruct-AWQ`
*   **Details:** [Hugging Face Model Card](https://huggingface.co/Qwen/Qwen2.5-VL-32B-Instruct-AWQ)
