# Text-to-fluid-Animation-Diffusers
Prompt and image interpolation using Diffusers to create smooth animations from a text.

The pipeline blends both the **text prompts** and the **images** to produce a coherent morphing effect, creating an artistic video that evolves from one verse to the next.

---

## Project Structure  
- **`text_to_animation.ipynb`**: Colab-ready notebook to generate the full video from a list of textual prompts  
- **`exemple.mp4`** : an exemple of what this notebook can produce 

---

## Technologies Used  
- **Python 3.11**
- **diffusers** (`StableDiffusionImg2ImgPipeline`)
- **MoviePy**
- **Pillow**
- **NumPy**
- **TQDM**

---

## How to Run  
1. Open the notebook in [Google Colab](https://colab.research.google.com)
2. Define your poem:
```bash
poem = [
    "Under the pale moonlight, silence hums in silver tones.",
    "Shadows dance softly on the lake’s shimmering skin.",
    "The forest breathes, ancient and patient.",
    "Time dissolves into golden dust."
]
```
3. The notebook will:
   - Generate an image for each line
   - Create smooth interpolations between each using prompt blending + `img2img`
   - Export a final video: `video.mp4`

---

## Example Output  
![preview](exemple.mp4)
