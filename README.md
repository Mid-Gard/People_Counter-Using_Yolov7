# People Counter Using ML Using Yolo V7 from Openvino

> This is the main branch now which will use optimized Openvino Yolov7 model. All the other branches which were using original model has been archived.

## Features
- Added Label for Every Track
- Code can run on Both (CPU & GPU)
- Video/WebCam/External Camera/IP Stream Supported
- Can store the footage for future reference in compressed format to save storage space and time.
- Also stores the data in text format.

## Steps to run Code
- Clone the repository.

- Goto the cloned folder: ``` cd UsingYolov7 ```

- Create a conda environment, as I was getting problem with installing dlib package using normal python. Its easier to install using conda.
  - Run following command : `conda create --name myenv python=3.8.18`
  - Ensure the evironment is activated : `conda activate myenv`.
  - Install all the packages in the environment : `pip install -r requirements.txt`.

- Give the IP address of the Camera in the `sources.txt` file.
  - You can add more links on new line, but the video wont be displayed, only result in terminal.

- Run the project: ``` python yolov7/detect.py ```


## TODO
1. Not able to display the frames, when using multicamera setup, only able to store the data. This may be due to the resolution variations of the different camearas used.
2. Need to create a good GUI, with better control features, will  able to show may be different camera footage on multiple boxes in same screen.
