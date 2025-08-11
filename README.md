## 📌 Project Overview
This project demonstrates **image generation using Stable Diffusion 2.1** with an additional **x2 Latent Upscale Pipeline** for enhanced realism.  
The chosen theme: **Photorealistic Night City Street in the Rain**.  
The goal is to explore how prompt complexity impacts the quality of generated images.

---

## 📂 Project Structure
diffusion-project

│── HM.ipynb # Jupyter Notebook with the generation code

│── README.md # Project description (this file)

│── requirements.txt # Python dependencies (auto-generated)

│── .gitignore # Excludes .venv and temporary files

└── IMG_FOR_TEST/ # Generated image examples


## 🛠 Technologies Used
- **Python 3.11**
- **PyTorch 2.6.0 + CUDA**
- **HuggingFace Diffusers**
- **Stable Diffusion 2.1**
- **Latent Upscale Pipeline (x2)**

---

## Example Results

**1️⃣ Simple prompt**  
`Photorealistic night city street in the rain`  
![city_01](IMG_For_Test/rain_city01.png)

**2️⃣ More detailed prompt**  
`Photorealistic night city street in the rain, wet asphalt reflecting neon lights, people with umbrellas walking along the sidewalk, realistic lighting and shadows`  
![city_02](IMG_For_Test/rain_city02.png)

**3️⃣ Highly detailed prompt**  
`Photorealistic night city street in the rain, wet asphalt reflecting colorful neon signs and streetlights, people with umbrellas walking along the busy sidewalk, shop windows glowing warmly, realistic lighting and shadows, cinematic composition, ultra realistic, high resolution, natural color grading, detailed reflections, physically based lighting, depth of field, 35mm photo, HDR`  
![city_03](IMG_For_Test/rain_city03.png)

---

## Observations & Conclusions
- More **descriptive prompts** produce more realistic and detailed results.  
- Using a **negative prompt** helps reduce artifacts, distortion, and oversaturation.  
- The **Latent Upscale Pipeline** improves micro-textures and overall sharpness.  
- The **most detailed prompt** provided the best visual quality in this test.

---

##  How to Run

### 1. Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/diffusion-model-homework.git
cd diffusion-model-homework
```

### 2. Create a virtual environment

```bash
python -m venv .venv
```

### 3. Activate the virtual environment

Windows (PowerShell):
```bash
.venv\Scripts\activate
```

macOS / Linux:
```bash
source .venv/bin/activate
```

### 4. Install dependencies

```bash
pip install -r requirements.txt
```

### 5. Run the Jupyter Notebook

```bash
jupyter notebook diffusion_task.ipynb
```
