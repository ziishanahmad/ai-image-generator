
```markdown
# AI Image Generator

## Overview

The **AI Image Generator** is a Python script that uses a pre-trained Stable Diffusion model to generate images from text prompts. This project leverages the power of the Stable Diffusion model to create high-quality images based on descriptive text inputs.

## Features

- Generate images from descriptive text prompts.
- Utilize the pre-trained Stable Diffusion model for high-quality image generation.
- Supports running on GPU if available, for faster processing.

## Prerequisites

Before you begin, ensure you have met the following requirements:

- You have installed Python 3.6 or higher.
- You have installed the necessary Python libraries: PyTorch, Hugging Face `diffusers` library, `transformers` library, and PIL (Python Imaging Library).

## Installation

To install the necessary libraries, follow these steps:

1. **Clone the Repository**

   Clone the repository to your local machine using the following command:

   ```sh
   git clone https://github.com/ziishanahmad/ai-image-generator.git
   cd ai-image-generator
   ```

2. **Install Required Libraries**

   Install the required libraries using `pip`:

   ```sh
   pip install torch diffusers transformers pillow
   ```

## Usage

To generate an image from a text prompt, follow these steps:

1. **Run the Script**

   Run the `generate_image.py` script using the following command:

   ```sh
   python generate_image.py
   ```

   This will generate an image based on the default prompt "mountain sunset" and save it as `generated_mountain_sunset.png`.

2. **Modify the Prompt**

   If you want to generate an image with a different prompt, modify the `prompt` variable in the script:

   ```python
   prompt = "your descriptive text here"
   ```

3. **Example**

   Here is an example of generating an image from the prompt "mountain sunset":

   ```python
   prompt = "mountain sunset"
   generated_image = generate_image_from_prompt(prompt)
   ```

   The generated image will be saved to the file `generated_mountain_sunset.png`.

## Example

Here is an example of generating an image from the prompt "mountain sunset":

1. **Text Prompt**

   ```sh
   "mountain sunset"
   ```

2. **Generated Image**

   ![Generated Image](ai-generated-image.png)

## AI-Generated Image

Here is an example of an AI-generated image:

![AI-Generated Image](ai-generated-image.png)

## Code Explanation

The main script `generate_image.py` performs the following steps:

1. **Import Libraries**

   The script imports necessary libraries such as `torch`, `transformers`, `diffusers`, and `PIL.Image`.

2. **Device Check**

   The script checks if a GPU is available and sets the device to CUDA if it is, otherwise it uses the CPU.

3. **Load Model**

   The Stable Diffusion model is loaded using the `StableDiffusionPipeline` from Hugging Face.

4. **Generate Image Function**

   The `generate_image_from_prompt` function takes a text prompt as input and generates an image using the Stable Diffusion model. It uses `torch.no_grad()` to avoid computing gradients, saving memory and computation.

5. **Example Usage**

   An example usage of the function is provided, generating an image from the prompt "mountain sunset" and saving it to a file.

## Contributing

Contributions are welcome! If you have any suggestions, bug reports, or feature requests, please open an issue or submit a pull request. 

To contribute:

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License. See the `LICENSE` file for more details.

---

**Author**: Zeeshan Ahmad

**GitHub**: [ziishanahmad](https://github.com/ziishanahmad)

**LinkedIn**: [Zeeshan Ahmad](https://www.linkedin.com/in/ziishanahmad/)
```
