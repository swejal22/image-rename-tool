# Image Rename Tool

## Description

The Image Rename Tool is a Python script that renames image files in a directory based on their metadata. It uses the exifread library to extract metadata from image files and allows you to specify a renaming pattern using the metadata fields such as date and time, camera model, and location.

## Features

- Extracts image metadata using the exifread library.
- Allows you to specify a custom renaming pattern using metadata fields.
- Renames multiple image files in a batch.

## Requirements

- Python 3.x
- exifread (install using `pip install exifread`)

## Installation

1. Clone or download this repository to your local machine.
2. Navigate to the project directory.
3. Install the required dependencies using the following command:

```bash
pip install -r requirements.txt
```

1. You will be prompted to enter the input directory path where your image files are located.
2. Next, you will be asked to provide the output directory path where the renamed images will be saved.
3. Optionally, you can specify a renaming pattern using the **{date_time}**, **{camera_model}**, and **{location}** placeholders. If no pattern is provided, the default pattern {date_time}_{camera_model} will be used.
4. The script will process all the image files in the input directory and rename them based on the specified pattern using the metadata information.
5. The renamed images will be saved in the output directory.

## Renaming Pattern

The renaming pattern can contain the following placeholders:

- **{date_time}:** Replaced with the date and time metadata from the image (e.g., "2023-08-03 12:34:56").
- **{camera_model}:** Replaced with the camera model metadata from the image (e.g., "Canon EOS 5D Mark IV").
- **{location}:** Replaced with the GPS location metadata from the image (e.g., "Latitude 40 deg 44' 58.00" N, Longitude 73 deg 59' 8.00" W").

## Note

- The script only supports image files with extensions .jpg, .jpeg, .png, and .gif.
- Ensure that the input and output directories exist before running the script.

## Contributing

Contributions are welcome! If you find any issues or have suggestions to improve the script, feel free to create an issue or submit a pull request.