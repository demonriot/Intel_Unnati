# Intel_Unnati
Detecting Pixelation in Images and Reconstruction of given Pixelated Images


<hr />

> **Implementation:** *a) Detecting pixelated images: Develop a lightweight, computationally efficient algorithm or ML/AI model to detect pixelated images with high accuracy (90%+) and low false positives, capable of processing 1080p resolution inputs at 60 Hz.b) Enhancing pixelated images: Create an algorithm to restore pixelated images, improving their quality while maintaining efficiency. The algorithm should not enhance non-pixelated images* 
<hr />


<p align="center">
  <img src = "https://private-user-images.githubusercontent.com/27466624/239739723-57391d0f-1848-4388-9f30-88c2fb79233f.jpg?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MjEwNTg1MTksIm5iZiI6MTcyMTA1ODIxOSwicGF0aCI6Ii8yNzQ2NjYyNC8yMzk3Mzk3MjMtNTczOTFkMGYtMTg0OC00Mzg4LTlmMzAtODhjMmZiNzkyMzNmLmpwZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA3MTUlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwNzE1VDE1NDMzOVomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTcxOWIzYjdkZTE3MGU2ZGM3OGZiZWRlNjk0NGNlMzgzYjNjZTdhYzg2M2M2OTExMDlhZmM2MDYzM2NjZmNjODEmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.SI-XoUL0BLMKU9DbVgOUyG_7qEPv2360QfwVWhJl7y0" width="700">
  <br/>
  <b> Overall Framework of MIRNet_v2 </b>
  This model is used for detecting pixelation in a given image
<br />
  A modified version of the CSPDarknet53 architecture forms the backbone of YOLOv8. This architecture consists of 53 convolutional layers and employs cross-stage partial connections to improve information flow between the different layers.

The head of YOLOv8 consists of multiple convolutional layers followed by a series of fully connected layers.
These layers are responsible for predicting bounding boxes, objectness scores, and class probabilities for the objects detected in an image.
One of the key features of YOLOv8 is the use of a self-attention mechanism in the head of the network.
This mechanism allows the model to focus on different parts of the image and adjust the importance of different features based on their relevance to the task.
Another important feature of YOLOv8 is its ability to perform multi-scaled object detection. The model utilizes a feature pyramid network to detect objects of different sizes and scales within an image.
This feature pyramid network consists of multiple layers that detect objects at different scales, allowing the model to detect large and small objects within an image.
</p>
<p align="center">
  <img src = "https://i.imgur.com/sX8Gubx.png" width="700">
  <br/>
  <b> Overall Framework of MIRNet_v2 </b>
  
  Given a degraded input image, image restoration aims to recover the missing high-quality image content. Numerous applications demand effective image restoration, e.g., computational photography, surveillance, autonomous vehicles, and remote sensing. Significant advances in image restoration have been made in recent years, dominated by convolutional neural networks (CNNs). The widely-used CNN-based methods typically operate either on full-resolution or on progressively low-resolution representations. In the former case, spatial details are preserved but the contextual information cannot be precisely encoded. In the latter case, generated outputs are semantically reliable but spatially less accurate. This paper presents a new architecture with a holistic goal of maintaining spatially-precise high-resolution representations through the entire network, and receiving complementary contextual information from the low-resolution representations. The core of our approach is a multi-scale residual block containing the following key elements: (a) parallel multi-resolution convolution streams for extracting multi-scale features, (b) information exchange across the multi-resolution streams, (c) non-local attention mechanism for capturing contextual information, and (d) attention based multi-scale feature aggregation. Our approach learns an enriched set of features that combines contextual information from multiple scales, while simultaneously preserving the high-resolution spatial details. Extensive experiments on six real image benchmark datasets demonstrate that our method, named as MIRNet-v2 , achieves state-of-the-art results for a variety of image processing tasks, including defocus deblurring, image denoising, super-resolution, and image enhancement.
</p>
<hr>
<b>Citations</b>
</hr>
<p>
 [1] @article{Zamir2022MIRNetv2,
title={Learning Enriched Features for Fast Image Restoration and Enhancement}, 
author={Syed Waqas Zamir and Aditya Arora and Salman Khan and Munawar Hayat 
        and Fahad Shahbaz Khan and Ming-Hsuan Yang and Ling Shao},
journal={IEEE Transactions on Pattern Analysis and Machine Intelligence (TPAMI)},
year={2022}
}    

[2]{cff-version: 1.2.0
title: Ultralytics YOLO
message: >-
  If you use this software, please cite it using the
  metadata from this file.
type: software
authors:
  - given-names: Glenn
    family-names: Jocher
    affiliation: Ultralytics
    orcid: 'https://orcid.org/0000-0001-5950-6979'
  - given-names: Ayush
    family-names: Chaurasia
    affiliation: Ultralytics
    orcid: 'https://orcid.org/0000-0002-7603-6750'
  - family-names: Qiu
    given-names: Jing
    affiliation: Ultralytics
    orcid: 'https://orcid.org/0000-0003-3783-7069'
repository-code: 'https://github.com/ultralytics/ultralytics'
url: 'https://ultralytics.com'
license: AGPL-3.0
version: 8.0.0
date-released: '2023-01-10'}
</p>
<hr>Data is in the 'master' branch<hr>
