# Real_time-emotion-recognition
Real-time face detection and emotion/gender classification using fer2013/imdb datasets and openCV.

It takes pictures or webcam video as input. It detects all faces in each frame, and then
    classifies which emotion each face is expressing.


It then replaces each face with an emoji corresponding to that emotion and according to emotion of person it will recommend the product which is suitable to that emotion from P&G products.


Recognized emotions:

        1. Neutral
        2. Happy
        3. Sad
        4. Angry
        5. Surprise
        6. Fear
 Training accuracy was 91% and test accuracy was 57%, with the following requirements:
        
        - User's facial expression must be strong / exaggerated
        - Lighting must be good (no shadows on face)
        - Camera is at eye level or slightly above eye level
  
  Requirements:
    
    > 2 GB of memory
    Caffe and OpenCV installed
    Webcam
        Note: Webcam currently does not work on virtual machines.
        Try using a native Mac or Linux system. Don't try on a virtual machine running on Windows.
        OpenCv and NumPy libraries installed.
        
     If you want to run on GPU:
        2GB or more VRAM
        CUDA and CuDNN libraries installed
        Caffe must be compiled with these CUDA and CuDNN selected


  Description of files:

    Main scripts:
  
      gather_training_data.py - Use this to generate a custom training set
      process_dataset.py - Read in an entire training set and calculate accuracy over the set
      process_image.py   - Read in a single image, add the correct emoji, and write to file
      video_generate.py  - Run in real-time and save output to video
      video_test.py      - Run in real-time; does not save to video

        
       
