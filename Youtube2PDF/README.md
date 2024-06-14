# YouTube to PDF Generator

This project provides a script to download a YouTube video, extract significant frames (scenes) based on structural similarity and histogram comparison, and compile these frames into a PDF. This tool is useful for creating a visual summary of a video, capturing key scenes, and presenting them in a document format.

## Features

- **Download YouTube Video**: Download the highest quality video from a given YouTube URL.
- **Scene Detection**: Extract key frames from the video using structural similarity index (SSIM) and histogram comparison to avoid duplicates.
- **PDF Creation**: Compile the extracted frames into a PDF document.
- **Progress Indicators**: Show progress bars for both downloading and processing phases.
- **Cleanup**: Automatically delete temporary image files after creating the PDF.

## Installation

1. **Clone the Repository**:
    ```bash
    git clone https://github.com/yourusername/your-repo-name.git
    cd your-repo-name
    ```

2. **Install Dependencies**:
    Make sure you have Python 3 installed. Then install the required libraries:
    ```bash
    pip install pytube opencv-python numpy scikit-image fpdf tqdm
    ```

## Usage

1. **Edit the Script**:
    - Replace the placeholder `YOUR_YOUTUBE_URL_HERE` with the actual YouTube URL you want to process in the script.

2. **Run the Script**:
    ```bash
    python youtube_to_pdf.py
    ```

3. **Check the Output**:
    - The script will generate a `scenes.pdf` file in the working directory containing the key frames from the video.

## Example

Here is an example of how to use the script:

```python
youtube_url = 'https://www.youtube.com/watch?v=example'  # Replace with your YouTube URL

