# jpgs-to-pdf
This repository contains a short Python script, that allows you to combine multiple JPG images into a single PDF document. The script utilizes the `fpdf` library for PDF generation and the `PIL` library for image manipulation.

To use the script, you need to provide the following inputs:

`-f` or `--folder`: The path to the folder containing the JPG images.

`-n` or `--name`: The desired name for the output PDF file.

`-e` or `--extension`: The extension of the image files to be considered (e.g., ".jpg", ".jpeg").

The script will recursively search the provided folder for image files with the specified extension and add them to a list. It will sort the images alphabetically and rotate any landscape mode images. Then, it will generate a PDF document by adding each image to a separate page using the dimensions of an A4 size sheet. The resulting PDF will be saved with the specified name in the input folder.

Please make sure you have the `fpdf` and `PIL` libraries installed before running the script.

Usage:

1. Clone the repository to your local machine.
2. Install the required dependencies by running `pip install fpdf Pillow`.
3. Open a terminal or command prompt and navigate to the repository directory.
4. Run the script with the following command:

```bash
python3 jpgtopdf.py -f /path/to/folder -n pdfname -e .jpg
```

Replace `/path/to/folder` with the path to the folder containing your JPG images, `pdfname` with the desired name for the output PDF file, and `.jpg` with the extension of your image files.
