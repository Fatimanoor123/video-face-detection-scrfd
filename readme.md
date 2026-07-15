# Video Face Detection using SCRFD

## Description
This project detects human faces in any uploaded video using the pretrained SCRFD model via InsightFace library. The pipeline processes each frame of the video, detects all faces, draws bounding boxes and facial landmarks, and saves the result as an output video.

## Pipeline
## Model
- **SCRFD** (Sample and Computation Redistribution for Efficient Face Detection)
- Pretrained model: `buffalo_l` via InsightFace
- Trained on millions of face images
- No training required — ready to use immediately

## For Each Detected Face, Model Returns
- **Bounding Box** → location of face [x1, y1, x2, y2]
- **Landmarks** → 5 key facial points (left eye, right eye, nose, mouth corners)
- **Confidence Score** → how sure the model is (0 to 1)

## Tech Stack
- Python
- OpenCV
- InsightFace
- ONNX Runtime
- Matplotlib
- Google Colab

## How to Run
1. Open notebook in Google Colab
2. Run all cells in order
3. Upload any video when prompted
4. Wait for processing to complete
5. Output video downloads automatically

## Results
- Detects multiple faces per frame
- Draws green bounding boxes around each face
- Marks 5 facial landmarks as red dots
- Shows confidence score per detected face
- Saves complete processed video

## Project Connection
This project implements Stage 2 and Stage 3 of the Bengali Celebrity Multimodal Dataset pipeline:

- **Stage 2** → Extract frames from video
- **Stage 3** → SCRFD detects faces in each frame

This pipeline is part of a larger research project to build a multimodal dataset of Bengali celebrities for speaker recognition — addressing a critical gap in South Asian AI research.

## Requirements
pip install insightface
pip install onnxruntime
pip install opencv-python
pip install matplotlib
## Sample Output
- Input  → any video with human faces
- Output → same video with green boxes around every detected face and red dots on facial landmarks
<img width="879" height="493" alt="image" src="https://github.com/user-attachments/assets/ca9680fd-1066-44b6-a701-2c44ef06a808" />

## Author
Fatima
Research Assistant 


## Acknowledgements
- [InsightFace](https://github.com/deepinsight/insightface)
- [SCRFD Paper](https://arxiv.org/abs/2105.04714)
- [OpenCV](https://opencv.org/)

## Related Projects
- [face-detection-scrfd]([https://github.com/fatima-noor-ai/face-detection-scrfd](https://github.com/Fatimanoor123/Face-Detection-SCRFD) → Face detection on images using SCRFD
