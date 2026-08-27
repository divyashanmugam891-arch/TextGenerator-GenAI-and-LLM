**🤖 AI Text Generator**

AI Text Generator is a simple web-based AI application created using Python, Streamlit, and Hugging Face Transformers.

This application allows the user to enter a sentence or short prompt and generate additional text using a pretrained language model.

**📌 About the Project**

The main purpose of this project is to understand how AI text generation works and how a pretrained Transformer model can be connected to a simple web application.

I used Streamlit to create the user interface and Hugging Face Transformers to generate text.

The application uses the Qwen/Qwen2.5-0.5B-Instruct pretrained model. The model is not trained from scratch in this project.

**✨ Features**

- ✍️ Enter a sentence or short prompt
- 🤖 Generate AI-based text
- ✨ Simple Generate Text button
- ⏳ Loading message while generating
- 📝 Display the generated text
- 🌐 Simple and easy-to-use Streamlit interface
- ⚡ Model caching for faster interaction

**🛠️ Technologies Used**

- Python
- Streamlit
- Hugging Face Transformers
- PyTorch
- Qwen/Qwen2.5-0.5B-Instruct

**⚙️ How It Works**

1. The user enters a sentence or prompt.
2. Streamlit receives the input.
3. The Qwen Transformer model processes the prompt.
4. The model generates additional text.
5. The generated text is displayed on the screen.


**🔄 Workflow**
```text
User Enters Prompt
        ↓
Streamlit Receives Input
        ↓
Qwen Transformer Model
        ↓
Text Generation
        ↓
Generated Text is Displayed
```


**🤖 Model**

This project uses the Qwen/Qwen2.5-0.5B-Instruct pretrained model.

The model is loaded using the Hugging Face Transformers pipeline:

from transformers import pipeline

```python
generator = pipeline(
    "text-generation",
    model="Qwen/Qwen2.5-0.5B-Instruct"
)
```


**🎛️ Text Generation Settings**

The application uses the following settings:

- Maximum new tokens: 40
- Number of sequences: 1
- Sampling: Enabled
- Temperature: 0.7
- Top-p: 0.9
- Repetition penalty: 1.1

These settings control how the AI generates the text.

**📦 Installation**

First, make sure Python is installed on your computer.

Install the required packages using:
```bash
pip install -r requirements.txt
```

The "requirements.txt" file contains:
```text
streamlit
transformers
torch
```


**▶️ Running the Application**

The Python file is saved as:
```text
textgen.py
```


Open the terminal in the project folder and run:
```bash
streamlit run textgen.py
```

The application will open in your browser.

The default Streamlit address is:
```text
http://localhost:8501
```


**🧪 Example**

Enter a prompt such as:

```text
Artificial Intelligence is
```

Then click the ✨ Generate Text button.

The model will generate additional text based on the given prompt.

The output may be different for different runs because sampling is enabled during text generation.

**📁 Project Structure**

```text
AI-Text-Generator/
│
├── textgen.py
├── README.md
├── requirements.txt
├── Capture.png
└── Textgen.png
```

**🎓 What I Learned**

Through this project, I learned about:

- AI Text Generation
- Transformer-based language models
- Hugging Face Transformers
- Pretrained AI models
- Streamlit
- Model caching
- Connecting an AI model to a web interface

**⚠️ Note**

The generated text may sometimes be incomplete, repetitive, or inaccurate.

The output can also be different for different runs because the model uses sampling.

This project is mainly created for learning and demonstration purposes.

**🚀 Future Improvements**

In the future, this project can be improved by adding:

- 🎛️ Temperature and token controls
- 🤖 Model selection
- 🧹 Clear or reset option
- 💾 Download option for generated text
- 📝 Prompt text-generation
- ration tasks

**👩‍💻 tasks**
AI Text GeneBuilt
Built using Python + Streamlit + Hugging Face Transformers.
