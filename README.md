# ConvNext-Implementation

Face Recognition (ResNet – 34) (Run Face Recognition.ipynb) <br>
Accuracy: 87.78% Implementation Details: <br>
• Embedding stem (3 -> 64) <br>
• 4 stages, 64 -> 128 -> 256 -> 512) <br>
• Optimizer – SGD with Nesterov <br>
• Loss – Cross entropy with label smoothing as 0.25 <br>
• LR Scheduler – Cosine Annealing (base LR = 0.1) <br>
Experimented with various augmentation techniques: <br>
1. Horizontal flip <br>
2. Random Augment <br>
3. Random Perspective <br>
4. Color Jitter <br>
Also calculated the mean and standard deviation of the training data separately to normalize all the values across the 3 channels. <br>

<br>
<br>

Face Classification (ConvNext) (Run Face Verification.ipynb) <br>
Verification Score (AUC): 0.96699 Implementation Details: <br>
• Embedding stem (3 -> 96) <br>
• Stages (96 -> 192 -> 384 -> 768) <br>
• Optimizer – SGD with Nesterov <br>
• Loss – Cross Entropy with label smoothing <br>
• Epochs - 55 <br>
Experimented with various augmentation techniques: <br>
1. Horizontal flip <br>
2. Random Augment <br>
3. Random Perspective <br>
4. Color Jitter <br>
5. Random Rotation <br>
6. Random Erasing <br>
