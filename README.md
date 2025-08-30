# DSPy Fun: Programmatic LLM and VLM use through DSPy

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/AdoHaha/dspy_fun/blob/main/programmatic_LLM_and_VLM_use_through_DSPy.ipynb)

An introduction to DSPy - a framework for programmatically solving tasks with large language models and vision language models.

**Author:** Igor Zubrycki  
**Email:** igorzubrycki@gmail.com

## What is DSPy?

DSPy is a framework that allows you to programmatically solve tasks with language models through:
- **Signatures**: Declarative specifications of input/output behavior
- **Modules**: Reusable components that can be composed together
- **Optimizers (Teleprompters)**: Automatic optimization of prompts and examples
- **Tool Integration**: Seamless connection with external APIs and databases

## Installation

```bash
pip install dspy opik
```

## What You'll Learn

This repository contains a comprehensive tutorial covering:

### 🚀 **Basic DSPy Usage**
- Using `dspy.Predict` for simple predictions
- Working with signatures and type constraints
- Handling different input types (text, numbers, images)

### 🎯 **Advanced Signatures**
- Creating custom signatures with detailed descriptions
- Optional output fields
- Type annotations and constraints

### 🔄 **Model Selection**
- Switching between different language models
- Cost considerations and optimization
- Using specialized models for specific tasks

### 🛠️ **Custom Modules**
- Building reusable components
- Combining strategies to fit your needs
- Chain of thought reasoning

### 🔍 **Tool Integration**
- Connecting external APIs and services
- Working with databases and vector stores

### 📚 **RAG (Retrieval-Augmented Generation)**
- Implementing retrieval strategies
- Reverse index search vs embedding-based search
- Integration with vector databases (ChromaDB)
- Using LangChain tools for file formats and databases
- Built-in FAISS support with `dspy.Embeddings`

### 🎛️ **Optimization & Training**
- Dataset preparation and requirements
- Metrics design and evaluation
- Using teleprompters for automatic optimization
- Judge models for evaluation

### 📊 **Logging & Monitoring**
- Integration with MLOps tools (Opik, MLFlow)
- Tracing information flow
- Cost and performance monitoring

## Files in this Repository

- **[Jupyter Notebook](programmatic_LLM_and_VLM_use_through_DSPy.ipynb)**: Interactive tutorial with hands-on examples
- **[PDF Presentation](programmatic%20LLM%20&%20VLM%20use%20through%20DSPy.pdf)**: Comprehensive presentation slides
- **README.md**: This overview and guide

## Getting Started

1. **Try it in Colab**: Click the Colab badge above to run the notebook directly in Google Colab
2. **Local Setup**: Clone this repository and install dependencies
3. **Follow Along**: Work through the notebook examples step by step

## Key Features Demonstrated

- **Multi-modal Support**: Work with text, numbers, and images
- **Flexible Input/Output**: Handle various data types and formats  
- **Optimization**: Automatic prompt and example optimization
- **Integration**: Connect with external tools and databases
- **Monitoring**: Track costs, performance, and information flow

## Example Usage

```python
import dspy

# Configure your model
model = dspy.LM("gemini/gemini-2.5-flash-lite", api_key=your_api_key)
dspy.configure(lm=model)

# Simple prediction
sum_of_numbers = dspy.Predict('numbers -> sum_of_numbers')
result = sum_of_numbers(numbers="12, 13, 15")
print(result)
```

## License

MIT License - see [LICENSE](LICENSE) file for details. Please pop me a message if you want to use the slides in your presentations. 
