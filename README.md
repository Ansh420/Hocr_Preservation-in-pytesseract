# Pytesseract with HOCR preservation

This is a fork of the Pytesseract library that preserves HOCR output. HOCR is a format for encoding the results of optical character recognition (OCR) in HTML. It is useful for preserving the layout of the original document and for further processing by other software.

To install this fork, simply run the following command:
# pip install pytesseract-hocr

Once installed, you can use the library in the same way as the standard Pytesseract library. 
However, to preserve HOCR output, you must set the hocr parameter to True when calling the image_to_string() function. 
For example:

import pytesseract

# Load the image
image = pytesseract.image.load('image.png')

# Recognize the text in the image, preserving HOCR output
text = pytesseract.image_to_string(image, hocr=True)

# Print the HOCR output
print(text)


This code will print the HOCR output to the console. 
You can then save the output to a file or process it further with other software.

<div class="ocr_page" id="page1">
  <div class="ocr_carea" id="carea1">
    <p class="ocr_par" id="par1">
      This is a sample of HOCR output. The text is wrapped in HTML elements that preserve the layout of the original document.
    </p>
  </div>
</div>


# Benefits of using HOCR output:

Preserves the layout of the original document
Can be processed further by other software
Is a standard format for encoding OCR results
Use cases for HOCR output:

# Creating searchable PDF files from scanned documents
Extracting text from images for further analysis
Archival purposes
Conclusion:

This fork of the Pytesseract library provides a convenient way to preserve HOCR output when performing OCR. 
This can be useful for a variety of tasks, such as creating searchable PDF files, extracting text for further analysis, and archival purposes.
