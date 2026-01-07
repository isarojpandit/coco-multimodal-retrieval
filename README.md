# coco-multimodal-retrieval

A Colab-friendly demo of **multimodal image–text retrieval** and **generation** on the COCO dataset using:

- **CLIP** for image/text embeddings  
- **FAISS** for efficient similarity search  
- **BLIP** for image captioning (image → text)  
- **Stable Diffusion** for text-to-image generation  

The notebook walks through building an end-to-end pipeline:

1. Download COCO validation images
2. Build embeddings and a FAISS index
3. Retrieve images from text queries (text → image retrieval)
4. Retrieve captions from images (image → text retrieval)
5. Generate new images with Stable Diffusion using the retrieved context

---

## Features

- 🔍 **Image retrieval from text** (COCO + CLIP + FAISS)  
- 🖼️ **Text retrieval from image** with BLIP captioning  
- 🎨 **Text-to-image generation** with Stable Diffusion (`runwayml/stable-diffusion-v1-5`)  
- 🧪 Designed to run in **Google Colab** with minimal setup  

---

## Project structure

```text
.
├── notebooks/
│   └── main.ipynb              # Main Colab notebook with the full pipeline
├── requirements.txt            # Python dependencies (for local use)
├── README.md
├── .gitignore
└── LICENSE                     # Optional: choose your preferred license
