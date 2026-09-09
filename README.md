# 🎨 AI Image Generation Project

An end-to-end **AI Image Generation** project developed using Deep Learning and Generative AI techniques. The project combines text processing, text embeddings, GAN-based image generation, attention mechanisms, and a unified **Gradio web application**.

## 🚀 Project Overview

This project demonstrates different approaches to generating and conditioning images using AI.

The complete project is implemented in a Jupyter/Google Colab notebook and provides a **single Gradio web application** through which the implemented features can be accessed.

### Key Technologies

* Python
* TensorFlow / Keras
* PyTorch
* Hugging Face Transformers
* Stable Diffusion
* GANs
* Conditional GANs
* Cross-Attention
* CLIP / Text Embeddings
* Gradio
* NumPy
* Pandas
* Matplotlib
* Google Colab

---

## 📌 Tasks Covered

### Task 1 — Text-to-Image Generation

A text-to-image generation interface using a pretrained Stable Diffusion pipeline.

Users can provide a text prompt and generate an image based on the prompt.

**Input:** Text prompt
**Output:** AI-generated image

---

### Task 2 — Conditional GAN Image Generation

A Conditional GAN-based image generation system.

The generator is conditioned on class labels to generate images belonging to different categories.

**Input:** Class/shape label
**Output:** Generated image

---

### Task 3 — Text Preprocessing & Text Embeddings

This section processes text prompts and converts them into numerical representations using a pretrained text encoder.

The generated embeddings can then be used as conditioning information for image generation.

**Pipeline:**

```text
Text Prompt
     ↓
Tokenizer
     ↓
Text Encoder
     ↓
Text Embedding
```

---

### Task 4 — Dataset Analysis

This section performs analysis and visualization of the available image/text dataset.

The dataset is explored using Python data analysis and visualization libraries.

**Tools used:**

* Pandas
* NumPy
* Matplotlib

---

### Task 5 — Cross-Attention GAN

A GAN architecture enhanced with **Cross-Attention** is implemented to incorporate text information during image generation.

The model uses:

* Noise vector
* Class label
* Text embedding
* Cross-attention mechanism

to generate conditioned images.

**Pipeline:**

```text
Noise + Label + Text Embedding
              ↓
       Cross-Attention GAN
              ↓
        Generated Image
```

---

### Task 6 — Complete Text-to-Image Pipeline

The final pipeline integrates the major components of the project into one workflow.

```text
User Text Prompt
       ↓
Text Preprocessing
       ↓
Tokenizer
       ↓
Text Embedding
       ↓
Condition Generation
       ↓
GAN / Cross-Attention Generator
       ↓
Generated Image
```

This provides an integrated demonstration of a real-world text-to-image generation workflow.

---

# 🌐 Gradio Web Application

All implemented functionality is integrated into **one Gradio application**.

The application provides a unified interface instead of launching separate Gradio applications for individual components.

### Application Flow

```text
                    ┌─────────────────────┐
                    │   Gradio Web App     │
                    └──────────┬──────────┘
                               │
        ┌──────────────┬───────┴───────┬──────────────┐
        ↓              ↓               ↓              ↓
   Text-to-Image     Basic GAN     Text Embeddings  Dataset
        │              │               │              │
        └──────────────┴───────┬───────┴──────────────┘
                               ↓
                       Cross-Attention GAN
                               ↓
                     Complete Pipeline
```

---

# 🛠️ Setup Instructions

## 1. Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/YOUR_REPOSITORY.git
cd YOUR_REPOSITORY
```

## 2. Install Required Libraries

For Google Colab, run:

```bash
pip install -q gradio
pip install -q transformers
pip install -q diffusers
pip install -q accelerate
pip install -q torch torchvision
pip install -q tensorflow
pip install -q pandas numpy matplotlib
```

Depending on the notebook environment, additional packages may be required by the notebook.

---

## 3. Open the Notebook

The project notebook can be opened directly in:

**Google Colab**

Upload the `.ipynb` file and execute:

```text
Runtime → Run all
```

Make sure all cells execute successfully before using the Gradio application.

---

# 📂 Dataset Setup

The required dataset should be placed in Google Drive / Colab according to the paths used by the notebook.

For example:

```text
/content/custom_dataset/
```

The dataset folder may contain the required book cover images and other project data.

If trained model files are used, place them in the appropriate project folder as well.

Example:

```text
project/
├── custom_dataset/
├── models/
│   ├── model.keras
│   └── other_weights.keras
└── AI_Image_Generation.ipynb
```

### Google Drive Dataset

Dataset access link:

**[ADD YOUR GOOGLE DRIVE DATASET LINK HERE]**

> Make sure the Google Drive folder permission is set to **Anyone with the link → Viewer** before submitting the link.

---

# 📁 Repository Structure

```text
AI-Image-Generation/
│
├── AI_Image_Generation.ipynb
├── README.md
│
├── screenshots/
│   ├── gradio_home.png
│   ├── text_to_image.png
│   └── generated_image.png
│
├── models/
│   └── trained_weights/
│
└── custom_dataset/
    └── dataset_reference.txt
```

> Large datasets and model weights do not need to be uploaded directly to GitHub. They can be hosted on Google Drive and linked from the README/submission form.

---

# 🖼️ Screenshots

Add screenshots of the working Gradio application here.

### Gradio Application

![Gradio Application](screenshots/gradio_home.png)

### Text-to-Image Generation

![Text-to-Image](screenshots/text_to_image.png)

### Generated Output

![Generated Image](screenshots/generated_image.png)

---

# 🎥 Demo

Add your demo GIF/video link here:

**Demo:** [ADD YOUR DEMO LINK HERE]

---

# 🔗 Project Links

| Resource              | Link                                     |
| --------------------- | ---------------------------------------- |
| GitHub Repository     | **[ADD YOUR GITHUB REPOSITORY LINK]**    |
| Google Drive Dataset  | **[ADD YOUR GOOGLE DRIVE DATASET LINK]** |
| Gradio Demo           | **[ADD YOUR GRADIO DEMO LINK]**          |
| Google Colab Notebook | **[ADD YOUR COLAB NOTEBOOK LINK]**       |

---

# 💻 Hardware / Environment

Recommended environment:

* Google Colab
* GPU Runtime
* Python 3.x
* CUDA-compatible GPU for faster model execution

For large generative models, GPU execution is strongly recommended.

---

# ⚠️ Notes

* Run the notebook from the beginning using **Run all**.
* Make sure all required dependencies are installed.
* Ensure the dataset path matches the path expected by the notebook.
* Model weights should be placed in the correct directory.
* The Gradio application should be launched only after all required models and functions have been initialized.

---

# 👨‍💻 Project

**AI Image Generation using GANs, Text Embeddings and Cross-Attention**

This project demonstrates the integration of Generative AI, Deep Learning, NLP, and interactive web interfaces into a unified image generation system.
