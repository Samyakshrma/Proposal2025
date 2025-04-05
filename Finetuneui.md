Google Summer of Code 2024 Proposal: Gemma Model Fine-tuning UI

Personal Information

Name: Samyak SharmaEmail: sammi.bgas@gmail.comGitHub/Portfolio: https://github.com/samyakshrmaLinkedIn: https://linkedin.com/in/samyakshrma

Synopsis

The goal of this project is to develop a user-friendly web interface that enables users to fine-tune Gemma models on their datasets. The UI will be built using Streamlit or Gradio, allowing users to upload datasets, configure hyperparameters, visualize training progress, and download fine-tuned models. Additionally, optional integration with Google Cloud Storage and Vertex AI will be considered to facilitate scalable training for those requiring cloud-based solutions.

Benefits to the Community

Fine-tuning large language models (LLMs) often requires significant expertise and resources, limiting accessibility for many researchers and developers. By providing an intuitive UI, this project will democratize fine-tuning, enabling a broader range of users—including researchers, developers, and students—to customize Gemma models without extensive coding knowledge. This will enhance usability, reproducibility, and accessibility, fostering innovation across various applications such as chatbots, summarization tools, and domain-specific assistants.

Deliverables

1. Dataset Uploading

Support multiple formats: CSV, JSONL, text files.

Implement data validation and preprocessing, including missing value handling and tokenization for NLP datasets.

Provide data augmentation options (optional), such as synonym replacement and back translation for text-based data.

2. Hyperparameter Configuration

Allow users to adjust key hyperparameters (learning rate, batch size, epochs, dropout rate, etc.).

Provide sensible defaults based on empirical research and automatic recommendations based on dataset size.

Include explanations of how each hyperparameter affects the model’s training and inference.

3. Training Progress Visualization

Display real-time loss curves and evaluation metrics (accuracy, F1-score, perplexity, etc.).

Implement a comparison view to show results across multiple fine-tuning sessions.

Optionally show generated text samples during training to provide insight into model performance.

4. Model Download/Export

Provide model export options: TensorFlow SavedModel, PyTorch, GGUF.

Enable easy loading for local inference or deployment with Hugging Face’s Transformers library.

Support quantization for optimized inference performance on edge devices.

5. Google Cloud Integration (Optional)

Support data storage on Google Cloud Storage (GCS) with authentication and access control.

Enable training on Vertex AI for scalability, allowing users to leverage TPU/GPU instances.

Provide cost estimates for cloud training to help users manage expenses.

6. Documentation & Examples

Write comprehensive documentation with API references and FAQs.

Include step-by-step tutorials and example datasets for users to get started quickly.

Provide troubleshooting guides for common issues such as data formatting errors and overfitting.

Technical Details

The project will leverage:

Python for backend logic and model fine-tuning.

Streamlit/Gradio for an intuitive frontend interface.

TensorFlow/PyTorch for model fine-tuning and inference.

Matplotlib/Plotly for training visualization, including dynamic and interactive charts.

Google Cloud SDK (optional) for cloud-based training and storage.

Hugging Face's Transformers library for easier model management and pre-trained weights.

Timeline

Week

Milestone

1-2

Familiarization with Gemma models, Hugging Face, and UI frameworks. Design initial wireframes and establish dataset upload pipeline.

3-4

Implement dataset upload and validation functionality, including preprocessing and augmentation features.

5-6

Develop hyperparameter configuration module with intelligent suggestions and explanations.

7-8

Implement training process, real-time visualization, and session comparison feature.

9-10

Develop model export functionality, including quantization and optimized deployment options.

11-12

Cloud integration (optional) and rigorous testing with different datasets and model architectures.

13-14

Final testing, documentation, and submission, along with comprehensive user guides.

Expected Size of Project

175-350 hours

Skills Required

Python

Streamlit/Gradio

TensorFlow/PyTorch

Data preprocessing and augmentation

Hugging Face Transformers

(Optional) Google Cloud Platform, TPU/GPU optimization

Resources

[Gemma Model Documentation]

[Streamlit Documentation]

[Gradio Documentation]

[TensorFlow/PyTorch Tutorials]

[Hugging Face Transformers Guide]

[Google Cloud Platform Guides]

Future Work

Beyond GSoC, this project could be expanded to support:

Multi-user collaboration with authentication and model versioning.

Additional model architectures and fine-tuning options, including multi-modal models.

Deployment as a hosted service for broader accessibility with serverless inference options.

Integration with AutoML frameworks for automatic hyperparameter tuning and model selection.

Why Me?

I am a Computer Science undergraduate at Dayananda Sagar College of Engineering (2022–2026), with hands-on experience in building ML-powered systems and deploying real-time applications.

Relevant Experience:

Code-Collab: Built a real-time collaborative coding platform using FastAPI, WebSockets, and Redis. Implemented secure authentication (JWT, OAuth2) and seamless multi-user session handling.

AI Assistant with Azure: Developed a FastAPI-based assistant using Azure’s STT and TTS APIs, Dockerized for scalable deployment.

SMS Spam Detection: Designed a spam classification system using NLP techniques with Scikit-learn, NLTK, and a Naïve Bayes model.

MNIST from Scratch: Implemented a neural network using NumPy to classify handwritten digits, focusing on forward/backward propagation and manual gradient descent.

Smart India Hackathon 2024 (Winner): Engineered SCADA Topology Discovery system using Python, GNS3, and FastAPI with secure SNMP and SSH communication layers.

Skills Snapshot:

Languages: Python, JavaScript, Go

Frontend: HTMX, Streamlit

Backend: FastAPI, Flask, Gin

Databases: MongoDB, Firebase, PostgreSQL, MySQL

ML Tools: TensorFlow, PyTorch, NLTK

DevOps/Cloud: Docker, GitHub Actions, AWS, Azure

Data Visualization: Tableau

Achievements:

Winner of Smart India Hackathon 2024, out of 50+ teams

Runner-up at HACK-O-RAMA! (Feb 2024), among 35+ teams

With a strong background in developing full-stack applications, real-time systems, and machine learning pipelines—both from scratch and using modern libraries—I am confident in my ability to execute this project and contribute meaningfully to the open-source community.
