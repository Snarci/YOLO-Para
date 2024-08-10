# YOLO-Para A specialized YOLO architecture for Malaria Parasites

### Architecture Overview
<div align="center">
  <img src="https://github.com/Snarci/YOLO-SPAM/blob/main/content/SPAMv8_3H.png" width="50%" height="50%"/>
</div><br/>

### Features
* Simple to train architecture for efficient malaria detection 
* STATE-OF-THE-ART for parasite detection in [[`MP-IDB`](https://link.springer.com/chapter/10.1007/978-3-030-13835-6_7),[`IML`](https://im.itu.edu.pk/a-dataset-and-benchmark-for-malaria-life-cycle-classification-in-thin-blood-smear-images/),[`M5`](https://arxiv.org/pdf/2111.13656.pdf)]

### Visual Results
<div align="center">
  <img src="https://github.com/Snarci/YOLO-SPAM/blob/main/content/result.png" width="80%" height="80%"/>
</div><br/>

### Detection Performance Comparison

This table compares the detection performance of our proposed framework against the state-of-the-art on different datasets.

| Dataset | Species | Work | Reference Model | AP | Increase AP% |
|---------|---------|------|------------------|----|--------------|
| M5      | P. Falciparum | Sultani *et al.* (2022)~[1] | Faster R-CNN | 66.8 | - |
| M5      | P. Falciparum | Proposed Framework | YOLO Para SMP | **71.0** | **4.2** |
| MP-IDB  | P. Falciparum | Zedda *et al.*~[4] | YOLO SPAM++ | 84.6 | - |
| MP-IDB  | P. Falciparum | Proposed Framework | YOLO Para AP | **86.5** | **1.9** |
| MP-IDB  | P. Malariae | Zedda *et al.*~[4] | YOLO SPAM | 94.1 | - |
| MP-IDB  | P. Malariae | Proposed Framework | YOLO Para AP | **94.9** | **0.8** |
| MP-IDB  | P. Ovale | Zedda *et al.*~[3] | YOLO PAM | 94.4 | - |
| MP-IDB  | P. Ovale | Proposed Framework | YOLO Para SMP | **95.1** | **0.7** |
| MP-IDB  | P. Vivax | Zedda *et al.*~[4] | YOLO SPAM++ | 87.5 | - |
| MP-IDB  | P. Vivax | Proposed Framework | YOLO Para AP | **88.3** | **0.8** |
| IML     | P. Vivax | Proposed Framework | YOLO Pra SMP | **67.4** | - |



## Setup

Before using the code, make sure to follow these setup instructions:

### [STEP 1] Ultralytics Installation

Extract the "ultralytics" zip file and place it in your Python packages folder.

### [STEP 2]  Select Model Configuration

The full list of model configurations can be found in the "config" folder.

### [STEP 3]  Create Data Configuration

The full list of data configurations can be found in the "data" folder.

### [STEP 4]  Train a YOLO-SPAM model

A small usage example is provided in the `train_notebook.ipynb` notebook.

## Contributing

Feel free to contribute by adding more papers, improving code, or providing feedback. Open issues and pull requests are welcome!

## License

This project is licensed under the [MIT License](LICENSE).

## References
[1] Sultani *et al.* (2022),[Link to Paper M5](https://arxiv.org/pdf/2111.13656.pdf)  
[2] Zedda *et al.* (ICIAP MALARIA),[Link to Paper ICIAP](https://link.springer.com/chapter/10.1007/978-3-031-06430-2_30)
[3] Zedda *et al.* (YOLO PAM PAPER),[Link to Paper YOLO PAM](https://www.mdpi.com/2313-433X/9/12/266)
[4] Zedda *et al.* (YOLO SPAM PAPER),[Link to Paper YOLO SPAM](https://www.sciencedirect.com/science/article/pii/S1746809424003471)



