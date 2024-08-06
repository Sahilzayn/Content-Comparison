# Document Comparison Project

This project compares uploaded documents against a set of documents in a folder based on both text and visual features. It uses OCR for text extraction and a ResNet model for visual feature extraction.

## Installation

To run this project, you'll need to install the following dependencies:

| Package         | Command                 |
|-----------------|-------------------------|
| pytesseract     | `pip install pytesseract` |
| Pillow          | `pip install Pillow`      |
| sentence_transformers | `pip install sentence-transformers` |
| torch           | `pip install torch`      |
| torchvision     | `pip install torchvision` |

Additionally, make sure to have Tesseract OCR installed on your system. You can download it from [here](https://github.com/tesseract-ocr/tesseract).

## Usage

1. **Initialize and load the model:**
   - Load the necessary libraries and models, including Sentence Transformers for text embeddings, ResNet for visual features, and other utility libraries.

2. **Extract text from an image:**
   - Define a function to extract text from a single image using Tesseract OCR.

3. **Extract texts from a folder:**
   - Define a function to iterate through a folder of images and extract text from each image.

4. **Extract visual features:**
   - Define a function to extract visual features from an image using a pre-trained ResNet model.

5. **Compare documents:**
   - Define a function to compare the extracted text and visual features of the uploaded document against those from the folder, computing similarity scores.

## Example

To use this project, follow these steps:

1. **Prepare the documents:**
   - Place the documents you want to compare in a folder.
   - Ensure your uploaded document is ready for processing.

2. **Initialize the models:**
   - Load a pre-trained ResNet model and set up the necessary transformations for image preprocessing.

3. **Process and compare documents:**
   - Use the provided functions to extract text and visual features from both the uploaded document and the folder of documents.
   - Compare the uploaded document against each document in the folder, and compute similarity scores.

4. **View the results:**
   - The system will output the similarity scores for each document in the folder, indicating how closely they match the uploaded document.

## Contributing

Contributions are welcome! Please submit a pull request or open an issue to discuss changes.

## License

This project is licensed under the MIT License - see the LICENSE file for details.
