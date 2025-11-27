AI Face Generator using Stable Diffusion v1.5
This project is a Jupyter Notebook-based application that allows users to generate realistic human faces using the **Stable Diffusion v1.5** model. The interface is built with `ipywidgets`, providing a user-friendly way to input prompts, login to Hugging Face if needed, and display generated images.


 Features
* Generate photorealistic portraits of humans based on textual prompts.
* Optional Hugging Face token login for gated models.
* User-friendly interface with buttons and text boxes.
* Uses GPU if available for faster inference.
* Provides negative prompts to avoid low-quality or distorted outputs.



Requirements
* Python 3.8+
* Jupyter Notebook or Jupyter Lab
* GPU (optional but recommended for faster generation)

       
Installation
Install the required libraries:

```bash
pip install diffusers transformers accelerate torch ipywidgets huggingface_hub
```

---

Usage

1. **Open the Notebook** in Jupyter.
2. **Login to Hugging Face (Optional)**:

   * Enter your Hugging Face token in the prompt if you want access to gated models.
   * Click **Login**.
3. **Load the Model**:

   * Click **Load Model** to initialize Stable Diffusion v1.5.
   * Wait for confirmation that the model is loaded.
4. **Generate Faces**:

   * Enter a description of the face in the **Prompt** box (e.g., "a smiling young woman with brown hair").
   * Click **Generate Face**.
   * The generated image will be displayed below.

---
Code Overview

1. **Library Imports and Device Setup**:

   * Imports PyTorch, diffusers, Hugging Face login, IPython display, and PIL.
   * Detects GPU availability automatically.
2. **Hugging Face Login UI**:

   * Optional step to login for access to private or gated models.
3. **Model Loading**:

   * Loads `runwayml/stable-diffusion-v1-5` using `EulerDiscreteScheduler`.
4. **Face Generation**:

   * Takes user prompt, applies styling and negative prompts.
   * Generates a photorealistic face and displays it.



Example Prompt

* `"a smiling young woman with brown hair"`
* `"an elderly man with glasses and a beard"`
* `"a child with curly hair and freckles"`


Notes

* Generation speed depends on your system and GPU availability.
* Negative prompts help reduce artifacts and unrealistic outputs.
* Always use safe and ethical prompts.


Output-
       


Acknowledgements

* [Hugging Face](https://huggingface.co/)
* [Stable Diffusion](https://github.com/CompVis/stable-diffusion)
* [Diffusers Library](https://github.com/huggingface/diffusers)
