# GroundingDINO-Inference
This project represents a GroundingDINO Inference (zero-shot object detection) procedure with both methods (CLI and Script). This implementation will help the reader to know the sequence of commands and exemplifying commands for running a quick zero-shot object detection. Additionally, the reader may get insight into code (script) execution.  This is the Google Colab implementation and has some prerequisites for the complete execution of the script. 

Prerequisite:
The user would need a folder that should be uploaded on the drive. The link to the folder is https://drive.google.com/drive/folders/1ctzsamgcgQ9OpxclnNlj7iLYsbbbh2R3?usp=share_link. The user needs to download that folder and upload it to the drive.

1. [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1kX1IeVrwA9J97lN1MqsFF_afambuinv8#scrollTo=4dEL6xotpB_A)

2. [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1eJye4465EpEZ_h1loUcyPsPecKhhT9ka#scrollTo=KxbH9rKcHdjn)

## Demo Results

### Demo1

![](https://github.com/HassanBinHaroon/GroundingDINO-Inference/blob/main/Demo%20Images/img1.jpg)

### Demo2

![](https://github.com/HassanBinHaroon/GroundingDINO-Inference/blob/main/Demo%20Images/img2.jpg)

### Demo3

![](https://github.com/HassanBinHaroon/GroundingDINO-Inference/blob/main/Demo%20Images/annotated_image.jpg)

### Demo4

![](https://github.com/HassanBinHaroon/GroundingDINO-Inference/blob/main/Demo%20Images/annotated_image(1).jpg)

### Demo5

![](https://github.com/HassanBinHaroon/GroundingDINO-Inference/blob/main/Demo%20Images/annotated_image(2).jpg)

## Inference Steps:

### Step1

    from google.colab import drive
    drive.mount('/content/drive')

### Step2

    cd drive/MyDrive/GroundingDINO/

### Step3

    pip install -q -e .
    
### Step4
 
    python demo/inference_on_a_image.py -c groundingdino/config/GroundingDINO_SwinT_OGC.py -p weights/groundingdino_swint_ogc.pth -i frame1.jpg -o "output" -t "bike . person . car ." 

## Results Visualization

Go to the output folder that would be created automatically.

## Important Announcement

This is just the beginning of the project. More options and features may be provided in the future.
