# Basic Agent Langflow Demo

This demo showcases how to build a simple AI Agent on HPEs Private Cloud AI leveraging Langflow. The agent has two tools available to itneract with a PDF (RAG) and infromation in a Table (Presto). Langflow is used as imported Framework, Qdrant as VectorDB, ezPrestoMCP Server (for AIE 1.12 and above) or custom written component to interact with the database information.
We provide two flavors of the demo, the flight assistant agent and the citizen passport support agent. You can easily switch between those two datasets or even use your own. You will require a PDF and a CSV file.

---

### Context on Customer and Use Case

This demo is ideal for customers looking to build AI agentic workflows with NO-CODE LOW-CODE.

### Solution Overview and Demo Video
- [Solution Overview]
- Demo Video

---

### Key Features

---

## Prerequisites

### 1. Models deployed in HPE Machine Learning Inference Software

This application requires the following models to be deployed and running in HPE Machine Learning Inference Software on HPE PCAI:

```yaml
required_models:
  - number: 1
    role: large_language_model
    name: Qwen/Qwen2.5-7B-Instruct
    source:
      provider: Hugging Face
      url: https://huggingface.co/Qwen/Qwen2.5-7B-Instruct

  - number: 2
    role: embedding_model
    name: nvidia/nv-embedqa-e5-v5
    source:
      provider: NVIDIA
      url: https://build.nvidia.com/nvidia/nv-embedqa-e5-v5
      
