# MKV to MP4 Converter

This Jupyter Notebook provides a solution for converting video files from MKV format to MP4 format using the `ffmpeg` library in Python. This conversion retains video quality while producing a widely compatible MP4 output, suitable for most devices and media players.

## Features
- **Batch Conversion**: Converts all MKV files within a specified directory to MP4.
- **Quality Retention**: Utilizes FFmpeg for high-quality video encoding.
- **Automated Directory Creation**: Saves converted MP4 files in a new output directory, preventing overwrites and keeping files organized.

## Requirements
- **FFmpeg**: This tool is essential for video conversion. The notebook includes a cell that installs FFmpeg if it’s not already present.
- **Python Libraries**:
  - `os`: For managing file and directory operations.
  - `subprocess`: To execute FFmpeg commands within Python.

## Usage
1. **Setup**: Open the notebook in Jupyter and execute the initial cells to ensure FFmpeg is installed.
2. **Specify Directories**:
   - Set the `input_folder` variable to the directory containing your MKV files.
   - The script automatically creates an `output_folder` to store the converted MP4 files.
3. **Run the Conversion**: Execute the conversion cell, which processes all MKV files in the input directory and saves the MP4 versions in the output directory.

### Example Usage
```python
input_folder = 'path/to/your/mkv/files'  # Replace with your MKV directory
output_folder = 'path/to/save/mp4/files' # Replace with your desired output directory
```

Once these paths are set, running the conversion code block will convert each MKV file in the specified directory.

## Troubleshooting
**FFmpeg Not Found**: If FFmpeg installation fails, ensure that Jupyter has the required permissions to install packages.
**File Access Issues**: Make sure you have read/write permissions for the input and output directories.

# License
This project is open-source and freely available for modification and use.
