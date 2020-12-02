# Person Detection on Raspberry Pi (Tecare)

## Using Tensorflow Lite

1. Install all system dependencies
2. Install python dependencies `pip3 install -r requirements.txt`
3. Run video scripts `python TFLite_detection_video.py --video=videos/fall_benchmark.mp4 --modeldir=ssd_mobilenet_model --threshold=0.1 --gap=20`

### Params
--gap: number of frames after last person detected to keep sending the video
--modeldir: model folder containing .tflite and .txt
--threshold: confidence threshold for machine learning model to consider true
--video: path for video file

*Only TFLite_detection_video.py supports detection on angle 0, 90, 180 and 270 deg

*Credit: https://github.com/EdjeElectronics/TensorFlow-Lite-Object-Detection-on-Android-and-Raspberry-Pi