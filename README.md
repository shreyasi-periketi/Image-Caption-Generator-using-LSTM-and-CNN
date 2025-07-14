# Image Caption Generator using LSTM and CNN

This project focuses on building an Image Caption Generator, a deep learning model that generates natural language descriptions for images. It combines a Convolutional Neural Network (CNN) for extracting image features and a Long Short-Term Memory (LSTM) network for generating text sequences.

Using a dataset of over 8,000 images from Flickr, each paired with 5 captions, the model learns to recognize visual elements and describe them in meaningful, grammatically correct sentences. Features from the image (via VGG16 or ResNet50) are fed into the LSTM, which then generates a caption word by word.

We evaluated the performance using BLEU scores, and achieved:
- VGG16:
  - BLEU-1: 0.5385
  - BLEU-2: 0.3222
- ResNet50:
  - BLEU-1: 0.5674
  - BLEU-2: 0.3415

These results show that the model effectively captures key elements in images, though like many neural networks, it may struggle with subtle details, abstract context, or creative language. Challenges include dataset limitations, language ambiguity, and model interpretability.

## Future Work
- Switch to Vision Transformer (ViT) + Transformer decoder for state‑of‑the‑art performance.
- Train/finetune on larger datasets (MS‑COCO, Conceptual Captions).
- Add beam search or nucleus sampling for more diverse captions.
- Explore attention heatmaps for interpretability.
- Deploy as a streamlit or FastAPI demo app.
