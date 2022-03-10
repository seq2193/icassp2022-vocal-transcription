# PSEUDO-LABEL TRANSFER FROM FRAME-LEVEL TO NOTE-LEVEL IN A TEACHER-STUDENT FRAMEWORK FOR SINGING TRANSCRIPTION FROM POLYPHONIC MUSIC
The source code of *"PSEUDO-LABEL TRANSFER FROM FRAME-LEVEL TO NOTE-LEVEL IN A TEACHER-STUDENT FRAMEWORK FOR SINGING TRANSCRIPTION FROM POLYPHONIC MUSIC"*, ICASSP2022


## Abstract

Lack of large-scale note-level labeled data is the major obstacle to singing transcription from polyphonic music. We address the issue by using pseudo labels from vocal pitch estimation models given unlabeled data. The proposed method first converts the frame-level pseudo labels to note-level through pitch and rhythm quantization steps. Then, it further improves the label quality through self- training in a teacher-student framework. 

<img src="./img/ICASSP2022-fig1-2.png" width="70%">

To validate the method, we conduct various experiment settings by investigating two vocal pitch estimation models as pseudo-label generators, two setups of teacher-student frameworks, and the number of iterations in self-training. The results show that the proposed method can effectively leverage large-scale unlabeled audio data and self-training with the noisy student model helps to improve performance. Finally, we show that the model trained with only unlabeled data has comparable performance to previous works and the model trained with addi- tional labeled data achieves higher accuracy than the model trained with only labeled data.


## Dependencies

- OS: LINUX 
- Programming language: Python 3.6+
- Python Library 
  - Keras 2.7.0 (Deep Learning library)
  - tensorflow 2.5.0 (Deep Learning library)
  - Librosa 0.8.1 (for STFT)  
  - pydub 0.25.1 (for loading audio and resampling)
  - pretty-midi (for handling midi data)
  - Numpy, SciPy

- Hardware
  - 1 GPU : GeForce GTX 3080ti
