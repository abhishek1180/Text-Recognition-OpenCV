### Deep Learning based Text Recognition (OCR) using Tesseract and OpenCV
Recognizing text in images using an open source tool called Tesseract and OpenCV. The method of extracting text from images is also called Optical Character Recognition (OCR)

In version 4, Tesseract has implemented a Long Short Term Memory (LSTM) based recognition engine. LSTM is a kind of Recurrent Neural Network (RNN). Version 4 of Tesseract also has the legacy OCR engine of Tesseract 3, but the LSTM engine is the default. We can use this tesseract tool to perform OCR on images and the output is stored in a text file.

pytesseract does not provide true Python bindings. Rather, it simply provides an interface to the tesseract binary. The library is writing the image to a temporary file on disk followed by calling the tesseract binary on the file and capturing the resulting output. This is definitely a bit hackish, but it gets the job done for us.pip install pillow pip install pytesseract pip install tesseract pip install easydict
