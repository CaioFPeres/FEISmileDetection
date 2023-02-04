# FEI Smile Detection

This is a project for detecting smiles, using the FEI face dataset, folder b (subjects smiling). I manually tightly annotated every smile on the images, and converted the original images to PNG for better overall training performance.

Achieved with Dlib's MMOD (deep learning) in C++. Several runs were conducted in order to find the best detector window.
FEI dataset provides 200 images with smiling subjects, but some of them were discarded, resulting in 190 images.

I didn't select a testing group in this project, but evaluated the model using myself with a webcam, and although we had access to a small number of images, it achieved good performance.

Most of the time, detections would be smaller on width than the annotated bounding boxes. Maybe tighting the bounding boxes wasn't a good idea.