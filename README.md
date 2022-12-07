# ConvNext-Implementation

Face Recognition (ResNet – 34) (Run Face Recognition.ipynb)
Accuracy: 87.78% Implementation Details:
• Embedding stem (3 -> 64)
• 4 stages, 64 -> 128 -> 256 -> 512)
• Optimizer – SGD with Nesterov
• Loss – Cross entropy with label smoothing as 0.25
• LR Scheduler – Cosine Annealing (base LR = 0.1)
Experimented with various augmentation techniques:
1. Horizontal flip
2. Random Augment
3. Random Perspective
4. Color Jitter
Also calculated the mean and standard deviation of the training data separately to normalize all the values across the 3 channels.


Face Classification (ConvNext) (Run Face Verification.ipynb)
Verification Score (AUC): 0.96699 Implementation Details:
• Embedding stem (3 -> 96)
• Stages (96 -> 192 -> 384 -> 768)
• Optimizer – SGD with Nesterov
• Loss – Cross Entropy with label smoothing
• Epochs - 55
Experimented with various augmentation techniques:
1. Horizontal flip
2. Random Augment
3. Random Perspective
4. Color Jitter
5. Random Rotation
6. Random Erasing
