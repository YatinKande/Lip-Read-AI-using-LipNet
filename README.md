# Lip-Read AI using LipNet 🗣️

This project implements lip reading using a LipNet-inspired deep learning model. LipNet is designed to recognize spoken words from silent video sequences of lip movements, using spatiotemporal convolutions and recurrent layers for end-to-end sentence-level prediction.

## Features

- End-to-end sentence-level lip reading
- Deep learning model based on 3D CNNs (spatiotemporal convolutions) and Bidirectional LSTMs
- Uses CTC loss for variable-length transcription
- Preprocessing and data augmentation for video inputs
- Robust data pipeline for video alignment and labeling
- Ready-to-use scripts for training and inference

## Real-World Use Cases

- **Accessibility:** Assists individuals who are deaf or hard of hearing by converting lip movements to text.
- **Noisy Environments:** Recognizes speech when audio is unreliable or unavailable (e.g., in factories, concerts, or busy streets).
- **Silent Communication:** Enables communication where speaking aloud is impractical, such as libraries or surveillance operations.
- **Security and Surveillance:** Supports video monitoring to interpret conversations without audio.
- **Video Conferencing:** Improves transcription in online meetings when audio is unclear or muted.

## Installation

1. Clone the repository:
    ```
    git clone https://github.com/YatinKande/Lip-Read-AI-using-LipNet.git
    cd Lip-Read-AI-using-LipNet
    ```
2. Install dependencies:
    ```
    pip install tensorflow opencv-python numpy matplotlib imageio gdown pandas jupyter
    ```

## Usage

1. Prepare your video dataset following the required format in the `data/` folder.
2. Run the Jupyter notebook for training and prediction:
    ```
    jupyter notebook LipNet_DL_Project_Final.ipynb
    ```
3. (Optional) For script-based workflows, you could implement similar scripts as `train.py` and `predict.py`:
    ```
    python train.py --data_dir /path/to/dataset
    python predict.py --video /path/to/video.mp4
    ```

## Directory Hierarchy

|—— app  
|—— data  
|     |—— s1 (video files)  
|     |—— alignments (text alignments)  
|—— models  
|—— output  
|—— LipNet_DL_Project_Final.ipynb  
|—— .gitignore  
|—— README.md  

## References

- [LipNet: End-to-End Sentence-level Lipreading](https://arxiv.org/abs/1611.01599)
- [Original LipNet Implementation](https://github.com/rizkiarm/LipNet)
- GRID dataset for training and testing

## License

This project is licensed under the MIT License. See the LICENSE file for more details.
