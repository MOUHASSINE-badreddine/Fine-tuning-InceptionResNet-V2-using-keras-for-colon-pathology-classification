# Fine-tuning-InceptionResNet-V2-using-keras-for-colon-pathology-classification

## Introduction
  > We used the Chaoyang dataset that contains Colon slides for fine tuning Inception-ResNet-V2 using keras to classify wich of those pathologies are normal, serrates, adenoma or adenocarcinoma.

## Dataset
<img src="https://i.ibb.co/nQMv3Q5/image.png" alt="image">
  > The dataset includes Colon slides from Chaoyang hospital, the patch size is 512 × 512. Training set contains 1111 normal, 842 serrated, 1404 adenocarcinoma, 664 adenoma samples, and testing set contains 705 normal, 321 serrated, 840 adenocarcinoma, 273 adenoma samples.
  The dataset is related to the following paper [Hard Sample Aware Noise Robust Learning for Histopathology Image Classification](https://ieeexplore.ieee.org/document/9600806)

## Usage
  * First you need to install the required packages using the following command:
    ```sh
      pip install -r requirements.txt
    ```
  * Then, you use the following command to start trainig and saving the model:
    ```sh
      main.py --baseDirectory --batchsize --epochs --savingDirectory
    ```
   * For help use: 
   ```sh
      main.py -h
   ```
## Reference

  ```
  @article{zhuhard,
    title={Hard Sample Aware Noise Robust Learning for Histopathology Image Classification},
    author={Zhu, Chuang and Chen, Wenkai and Peng, Ting and Wang, Ying and Jin, Mulan},
    journal={IEEE transactions on medical imaging}
  }
  ```
