# README

## Project: Image Generation using Stable Diffusion

### Overview
This project demonstrates how to generate images using the Stable Diffusion model, a state-of-the-art deep learning model for text-to-image generation. The script utilizes the `diffusers`, `transformers`, and `torch` libraries to create and save multiple images based on a given textual prompt.

### Prerequisites

Before running the script, ensure you have the following libraries installed:

- `diffusers`
- `transformers`
- `torch`
- `accelerate`
- `matplotlib`

You can install the required libraries using pip:

```bash
!pip install diffusers transformers torch accelerate matplotlib
```

### Script Breakdown

1. **Library Imports**: 
   The script begins by importing the necessary libraries, including `diffusers` for the Stable Diffusion pipeline, `torch` for managing GPU resources, `os` for file management, and `matplotlib` for displaying images.

2. **GPU Setup**:
   The script checks if a GPU is available using `torch.cuda.is_available()`. If a GPU is available, the model will run on it; otherwise, it defaults to the CPU.

3. **Loading the Stable Diffusion Model**:
   The model is loaded using the `StableDiffusionPipeline` from the `diffusers` library. The `model_id` points to the pre-trained Stable Diffusion model (v1.4) available from the `CompVis` repository.

4. **Defining the Text Prompt**:
   A textual prompt is provided, which the model uses to generate images. In this example, the prompt describes a fantastical cityscape.

5. **Image Generation**:
   The script generates a specified number of images (`num_images`) based on the prompt. Each generated image is stored in the `images` list.

6. **Saving and Displaying Images**:
   The generated images are saved in the specified output directory (`/content/sample_data`). The images are also displayed using `matplotlib`.

### Usage

To use this script, follow these steps:

1. **Clone the Repository**:
   Clone this repository to your local machine or set up a Google Colab notebook.

2. **Install Dependencies**:
   Ensure all dependencies are installed using pip.

3. **Run the Script**:
   Execute the script in your preferred Python environment. It will generate and save the images to the specified output directory.

4. **View Generated Images**:
   The script will display the generated images inline, and they will also be saved as PNG files in the output directory.

### Example Output

The script will generate three images based on the given prompt, displaying them inline and saving them as `image_1.png`, `image_2.png`, and `image_3.png` in the `sample_data` directory.

### Customization

- **Prompt**: Modify the `prompt` variable to change the theme or subject of the generated images.
- **Number of Images**: Adjust the `num_images` variable to generate more or fewer images.
- **Output Directory**: Change the `output_dir` variable to save images to a different directory.

### Notes

- The quality and content of the generated images are highly dependent on the provided text prompt.
- Running the model on a GPU is recommended for faster image generation.

### Conclusion

This script provides a straightforward approach to generating images using the Stable Diffusion model. By tweaking the prompt and other parameters, you can explore a wide range of creative possibilities.

### License

This project is licensed under the MIT License. See the LICENSE file for more details.

---

**Author**: Ntokolo Thabants’o 
**Date**: Sat 24 August  
**Contact**: https://discord.com/invite/6XARWzh9
