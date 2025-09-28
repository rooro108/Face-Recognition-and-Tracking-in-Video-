# Face-Recognition-and-Tracking-in-Video-
For this project, I developed a system that can detect and recognize faces in a video and track how long each person appears on screen. The goal was to monitor individuals’ presence, log their appearance and disappearance times, and record the duration they stay visible

The dataset used consisted of images of known individuals, stored in separate folders per person. For example, one folder for “Ali” and another for “Sara,” each containing several face images. These images serve as references for recognizing people in the video. The input video can be any recorded footage where we want to detect and track people.
The system uses MTCNN for face detection and InceptionResnetV1 (pretrained on VGGFace2) for creating facial embeddings. Each detected face is compared with the known faces using cosine similarity. If the similarity exceeds a set threshold, the person is recognized; otherwise, they are marked as unknown.
The main features include:
1-Real-time detection and recognition of both known and unknown faces.
2- Logging of each person’s appearance, disappearance, and the time they remain in view.
3- Annotated video output with bounding boxes and labels for each face.
4- A CSV log containing all events for easy review.
This system is useful for monitoring attendance, analyzing movement patterns, or security purposes, providing both a visual record in video and a structured log for further analysis.
Dataset  : https://drive.google.com/drive/folders/1r2Fncm0o7QTWONVc5Bx4m3Sumgs-dHbE?usp=sharing

