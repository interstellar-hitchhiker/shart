# Shart
# Hexadecimal to Abstract Art: https://interstellar-hitchhiker.github.io/shart/

This project converts a user-inputted text into a unique piece of abstract art by mapping the SHA-256 hash of the text to various shapes, colors, and positions. The generated art is consistent for the same input text, ensuring that the same text always produces the same abstract image.

## Features

- **Text to Abstract Art**: Converts any text input into a unique piece of abstract art.
- **Consistent Output**: The same input text will always generate the same abstract art.
- **Downloadable Art**: Users can download the generated abstract art as a PNG image.
- **Interactive UI**: Simple and intuitive user interface for inputting text and generating art.

## Technologies Used

- **HTML**: Structure of the webpage.
- **CSS**: Styling of the webpage.
- **JavaScript**: Logic for converting text to hash, generating shapes, and rendering the art.
- **p5.js**: Drawing library used for rendering the abstract art.
- **js-sha256**: Library used for generating SHA-256 hash of the input text.

## Usage

1. **Input Text**: Type any text into the input field.
2. **Generate Art**: Click the "Generate Abstract Art" button to create the abstract art.
3. **View Hash**: The SHA-256 hash of the input text will be displayed below the input field.
4. **Download Art**: Click the "Download Image" button to save the generated abstract art as a PNG file.

## Installation

1. Clone the repository:

```bash
git clone https://github.com/yourusername/hexadecimal-to-abstract-art.git
Navigate to the project directory:
bash
Copy code
cd hexadecimal-to-abstract-art
Open the index.html file in your preferred web browser:
bash
Copy code
open index.html
Code Explanation

HTML
The structure includes an input field for the text, a display for the hash, and buttons to generate art and download the image.
A canvas element is used to draw the abstract art.
CSS
Styles the page for a clean and simple user interface.
Positions the elements centrally on the page.
JavaScript
Uses p5.js to handle the drawing of shapes on the canvas.
Uses js-sha256 to compute the SHA-256 hash of the input text.
Maps hexadecimal values of the hash to determine the shapes, colors, positions, and rotations.
Functions
setup(): Initializes the p5.js environment.
updateHash(): Updates the displayed hash when the input text changes.
hexToR(hex), hexToG(hex), hexToB(hex): Converts hex values to RGB colors.
generateImage(): Draws shapes on the canvas based on the hash values.
downloadImage(): Downloads the canvas content as a PNG file.
