## Facial Verification with a Siamese Network

**Project description:** This facial verification app utilizes a Siamese network to verify images against an anchor image. Developed in Google Colab and employing TensorFlow, Keras, OpenCV-Python, Matplotlib, and tqdm, the app builds on the innovative methodology outlined in a scientific paper. The entire process, from data collection to model engineering and final deployment, is orchestrated seamlessly.

### 1. Automatic Creation of Folder Structures

A well-organized folder structure is automatically generated to streamline the handling of different data types, including positive images, negative images, and anchor images. This enhances the maintainability and scalability of the project.

### 2. Download and Uncompress Negative Images

The negative images essential for training are automatically downloaded and uncompressed from [UMass LFW dataset](http://vis-www.cs.umass.edu/lfw/lfw.tgz). This automation speeds up the data preparation phase.
![Downloading negatives](images/01_Facial_Verification/Downloading_negatives.JPG)

### 3. Javascript for Collecting Positives and Anchors

A custom JavaScript code is utilized to collect 400 images comprising positives and anchors. This tailored approach ensures that the data collection process is precisely aligned with the project's unique requirements.

### 4. Data Augmentation

Data augmentation techniques are applied to amplify the initial collection ninefold. This enrichment strengthens the model's ability to generalize from the training data to unseen faces.

### 5. Load and Preprocess Images

Images are loaded and preprocessed using OpenCV-Python and other tools. The preprocessing includes normalization and other essential transformations to make the images suitable for training the Siamese network.

### 6. Model Engineering as Specified in the Paper

The app's architecture follows the specific guidelines and structure detailed in the referenced scientific paper. The use of TensorFlow and Keras libraries ensures a robust and flexible implementation.

### 7. Training with Binary Cross-Entropy and Adam Optimizer

Training is conducted using the binary cross-entropy loss function and the Adam optimizer. These choices reflect the binary nature of the verification task and the need for efficient optimization.

### 8. Precision, Recall, and Visual Results

Evaluation metrics such as precision and recall, along with visual results, are presented using Matplotlib. This comprehensive analysis provides clear insights into the model's performance.

### 9. Saving Model

The trained Siamese network model is saved securely, enabling potential future deployment or further refinement.

### 10. Building a Python App in Visual Studio Code

The project culminates in building a Python app using Visual Studio Code. This app integrates the trained model, offering a user-friendly interface for real-world facial verification.
