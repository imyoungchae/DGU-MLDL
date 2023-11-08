# DGU-MLDL

This data is based on the data from a myoelectric sensor, known as MYO. MYO has eight sensors arranged to measure the movement generated in the muscles beneath the attached surface.

Each line in the data set contains values for all eight sensors, and since each sensor has eight values, it consists of 64 columns.
The 65th column classifies the gesture produced through this, with rock = 0, scissors = 1, paper = 2, ok = 3. Thus, it is structured as [8sensors][8sensors][8sensors][8sensors][8sensors][8sensors][8sensors][8sensors][GESTURE_CLASS].
Since the data I have prepared has predefined answers, it falls under supervised learning and I will use multi-class classification to classify the 64 sensor values, the X data, into one of the four gestures: rock, scissors, paper, and ok. For this, I plan to use the Logistic Regression, Decision Tree, and SVC algorithms that we learned in class. I will analyze each algorithm in terms of accuracy and the time it takes to learn.

Moreover, even for the same algorithm, I will set different parameters for each algorithm: for Logistic Regression, I will use different solvers; for Decision Tree, I will adjust the depth; and for SVC, I will use different kernels. I plan to train with nine different cases, three for each algorithm.
