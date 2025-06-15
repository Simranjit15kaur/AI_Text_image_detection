


# AI-Generated Image and Text Detection System

This project is a comprehensive AI-generated content detection system capable of analyzing both **images** and **text** to assess whether the input is likely to have been produced by artificial intelligence models. It uses a combination of deep learning, statistical analysis, image metadata inspection, and natural language processing techniques.

## Table of Contents

- [Features](#features)
- [Architecture Overview](#architecture-overview)
- [Installation](#installation)
- [Running the Application](#running-the-application)
- [File Structure](#file-structure)
- [How It Works](#how-it-works)
  - [Image Analysis](#image-analysis)
  - [Text Analysis](#text-analysis)
- [Example Outputs](#example-outputs)
- [Dependencies](#dependencies)
- [Use Cases](#use-cases)
- [Acknowledgements](#acknowledgements)
- [License](#license)
- [Author](#author)

## Features

### Image Analysis

- Deep feature extraction using pre-trained CNN (ResNet50)
- Noise pattern detection using Laplacian variance, FFT, and Local Binary Patterns (LBP)
- EXIF metadata analysis (camera model, software, GPS, timestamp)
- Statistical analysis (mean, standard deviation, skewness, kurtosis)
- Resolution and aspect ratio heuristics
- AI signature detection (e.g., software like MidJourney, Stable Diffusion)
- Generates visual bar chart and gauge for AI-likelihood

### Text Analysis

- Preprocessing pipeline with unicode normalization, URL/email stripping, and HTML removal
- AI watermark phrase detection (e.g., "as an AI language model")
- Repetitive token pattern analysis (bigram/trigram repetition)
- Sentence length perplexity check
- Formal writing pattern recognition
- Produces a confidence score from multiple heuristics

### Interface

- Simple and intuitive **Gradio** web interface
- Upload an image or input text and receive:
  - AI-generation confidence score
  - Component-wise breakdown
  - Visual analytics

---

## Architecture Overview

- **Backend**: Python, TensorFlow/Keras, OpenCV, NLTK, SciPy, scikit-image
- **Visualization**: Plotly
- **Frontend**: Gradio UI for real-time interaction
- **Models**:
  - ResNet50 for image feature extraction
  - Rule-based NLP for text pattern detection

---

## Installation
!pip install gradio tensorflow opencv-python-headless exifread nltk plotly scikit-image


### Clone Repository

```bash
git clone https://github.com/simranjit15kaur/AI_Text_image_detection.git
cd AI_Text_image_detection


## Author

**Simranjit Kaur**

- Final Year Student, AI & ML Enthusiast
- Specialized in Explainable AI, Deep Learning, and Digital Twins
- Project Lead for "AI Text and Image Detector"
- Contact: skaur6_be22@thapar.edu
- GitHub: [github.com/Simranjit15kaur](https://github.com/Simranjit15kaur)
