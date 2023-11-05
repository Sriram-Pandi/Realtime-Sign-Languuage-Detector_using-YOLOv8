Your name and the names of all of your group members:
Sriram Pandi
Srinivas Peri
Rushi shah

Your project description (same one you used for the email check-ins)

Project description used while check-in:

Our project aims to develop a computer vision-based system using deep learning model to recognize and translate sign language actions/motions into text. First, a custom dataset will be created with different sign language poses and labelled using labelling image package. The next step would be performing transfer learning against Tensor-flow object detection API to train the object detector leading the system to be a real-time Sign language detection device.

Modification:

The project description provided previosuly was the initial trial but once we started implementing the project due to machine resource issue (errors with CUDA,cudNN,version errors) we had to move on to YOLOv8.The approach was same except that we used YOLOv8 instead of Tensorflow.

It's a request to please consider the machine limitation and consdier the changes made.


The URL for your presentation:

https://drive.google.com/file/d/1PIjdm0jpLlExUUa7WTiB9j5Ntz-lhnQT/view?usp=share_link


The URL(s) for any other demo videos you might have:

https://drive.google.com/file/d/1JVduN5isb8IU6PLwzi8OQFFTzR-8nIlS/view?usp=share_link


Link to drive:

https://drive.google.com/drive/folders/1qotx5pugATPX3BzHUW42tYIebM_ailwF?usp=sharing


The project had more issues with dataset preparation and labelling and augmentation than the actual implementation. Most of the project time was utilised in implementating it thorugh Tensor flow. Despite the fact that we put lot of time trying to implement it with Tensorflow we had to move on to YOLOv8 object detection because of system resources and unable to access GPU even after trying multiple versions of Tensor flow, CUDA and cudNN and even tried changing OS to ubuntu. once the dateset was prepared, labelled it was straightly training the model with all the lables and once we obtained the weughts. we wrote a script to run it for real time detection.The dataset created along with the weights obtained were provided in the google drive link provided above.