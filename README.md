![Dataset](https://www.kaggle.com/datasets/toluwaniaremu/smartcity-cctv-violence-detection-dataset-scvd)


# System requirements and status

## For local runtime in Google Colab ( Docker ) 
- C3D, Resnet


## Setup the python 3.10.

```bash
$env:Path = "C:\Users\srsho\AppData\Local\Programs\Python\Python310;" + $env:Path
$env:Path = "C:\Users\srsho\AppData\Local\Programs\Python\Python310\Scripts;" + $env:Path

python --version

./venv/Scripts/Activate
```
### Error and Solution
- RuntimeError: Input type (torch.cuda.FloatTensor) and weight type (torch.FloatTensor) should be the same
- Solution:
 - put the weight in the device like model.to(device) in pytorch

### VideoResnet2
- Trained on 112x112 and 16 fps

