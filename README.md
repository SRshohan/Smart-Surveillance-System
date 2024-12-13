# Smart City CCTV Violence Detection Project

## Dataset
[SCVD (Smart City CCTV Violence Detection) Dataset](https://www.kaggle.com/datasets/toluwaniremu/smartcity-cctv-violence-detection-dataset-scvd)

## System Requirements

### Python Setup
- **Python Version**: 3.10
- **Virtual Environment Setup**:
  ```bash
  $env:Path = "C:\Users\srsho\AppData\Local\Programs\Python\Python310;" + $env:Path
  $env:Path = "C:\Users\srsho\AppData\Local\Programs\Python\Python310\Scripts;" + $env:Path
  
  python --version
  ./venv/Scripts/Activate
  ```

### Local Runtime (Google Colab with Docker)
- Supported Models:
  - C3D
  - ResNet

## Dependencies
- opencv-python
- matplotlib
- Keras-Preprocessing
- scikit-image
- tensorflow
- pandas
- torch

## Common Troubleshooting

### PyTorch Device Compatibility Error
**Error**: 
```
RuntimeError: Input type (torch.cuda.FloatTensor) and weight type (torch.FloatTensor) should be the same
```

**Solution**:
Ensure model and input are on the same device:
```python
model.to(device)
```

## Model Specifications

### VideoResnet2
- Training Resolution: 112x112
- Frame Rate: 16 fps

## Installation

1. Clone the repository
2. Set up virtual environment
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

