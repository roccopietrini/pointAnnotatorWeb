# pointAnnotatorWeb
Annotation tool for Amazon mTurk

This code can be used in Amazon Mturk to annotate points in images. In my case body joints to later train a neural network for detection.

Left mouse click to select a point, right click to skip it (in this case the coordinates are x=-1,y=-1). Change the label array to whaever to want to annotate, the labels are used only to guide the user, but its lenght is used to check if the work is complete (all point must be annotated) and activate the submit button. Output will be a single field Answer.coordinates in the result csv with this structure "x1,y1;x2,y2..xn,yn". The annotation order must be the same for all images and related to the labels array.

# Usage
Simply copy the code in the source layout of the amazon mturk proect, adjiust the label array and data-imgsrc variable according to the uploaded dataset.

# Aknowledgement
This work is inspired by the work of [TukoFernandes](https://github.com/TucoFernandes/ImaTil)
