# Real-Time Hand Sign Detection with YOLOv8

A notebook-based project for detecting labeled hand signs.

1. [Collect images](python_files/imgcollection.ipynb) with a camera if building your own dataset.
2. [Train the model](python_files/Yolov8_Sign_Language.ipynb) using the labeled dataset and its configuration.
3. [Run live inference](python_files/realtime.ipynb) by supplying model weights and updating the input source and weights path.

The dataset and weights are external to this repository. See the [project report](Project_report_PRCV.pdf) for the experimental setup.

## Reproduction checklist

Open the data collection notebook only if collecting new images. For training, check that the dataset YAML paths resolve and the class list matches the annotations. For live inference, set the checkpoint path and camera source and check a known sign before testing other classes. The report describes the original experiment, while local accuracy and speed depend on the dataset, checkpoint, and hardware.
