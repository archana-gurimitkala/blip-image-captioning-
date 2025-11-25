# BLIP Image Captioning

A simple implementation of image captioning using the BLIP (Bootstrapping Language-Image Pre-training) model from Salesforce.

## Overview

This project uses the `Salesforce/blip-image-captioning-base` model to generate descriptive captions for images. BLIP is a vision-language model that can understand and describe images in natural language.

## Features

- Generate captions for images using state-of-the-art BLIP model
- Simple and easy-to-use implementation
- Works with local image files

## Requirements

Install the required packages:

```bash
pip install transformers torch pillow
```

## Usage

1. Update the `image_path` variable in the notebook with the path to your image:
   ```python
   image_path = "path/to/your/image.jpg"
   ```

2. Run the notebook cells to:
   - Load the BLIP model and processor
   - Process your image
   - Generate and display the caption

## Example Output

```
Image Explanation:
 a lake surrounded by trees and a mountain
```

## Model Details

- **Model**: `Salesforce/blip-image-captioning-base`
- **Framework**: Hugging Face Transformers
- **Task**: Image Captioning

## How It Works

1. The BLIP processor prepares the image for the model
2. The BLIP model generates a sequence of tokens describing the image
3. The processor decodes the tokens into a readable caption

## Notes

- The model will be downloaded automatically on first use (requires internet connection)
- Model files are cached locally after the first download
- Processing time depends on your hardware and image size

## License

This project uses the BLIP model from Salesforce. Please refer to the model's license for usage terms.

## References

- [BLIP Paper](https://arxiv.org/abs/2201.12086)
- [Hugging Face Model Card](https://huggingface.co/Salesforce/blip-image-captioning-base)

