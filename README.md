## Colorizing Black and White Images
https://github.com/rimo10/Image-Colorization-Project/assets/70977847/5b3fa0c8-9c20-46f6-a518-6180d69f0305
## Tech Stack
* [PyTorch ](https://pytorch.org/) for Model Training <br>
* [Streamlit ](https://streamlit.io/) for making the web Application

## Datasets used
The following datasets were used to train the model
<br>
Base
1. [ImageNet 12k ](https://www.kaggle.com/datasets/lijiyu/imagenet)
 
Landscape
1. [Landscape Recognition | Image Dataset | 12k Images](https://www.kaggle.com/datasets/utkarshsaxenadn/landscape-recognition-image-dataset-12k-images)
2. [Landscape Pictures ](https://www.kaggle.com/datasets/arnaud58/landscape-pictures)
 
Person
1. [Human Faces ](https://www.kaggle.com/datasets/ashwingupta3012/human-faces)
2. [FFHQ Face Data Set ](https://www.kaggle.com/datasets/greatgamedota/ffhq-face-data-set) 

Fruits and Flowers
1. [Fruits 360 ](https://www.kaggle.com/datasets/moltean/fruits)

Animals
1. [Animals Detection Images Dataset ](https://www.kaggle.com/datasets/antoreepjana/animals-detection-images-dataset)

## Train your own model
You can use the pretrained weights avialable under `models` folder. Or if you want you can train on your own custom dataset 
1. Clone the repo `https://github.com/rimo10/Image-Colorization-Project.git`
2. Open `Image_Colorizer.ipynb` 
3. Copy the model path and run the cell - 
 
 ```python 
 def load_checkpoint(model,path):
     model.load_state_dict(torch.load(path)) 
     return model
     
 load_checkpoint(model,your_weights_path)
 ```
 
 ## To Run the Web App
 1. Clone the repo `git clone https://github.com/rimo10/Image-Colorization-Project.git`
 2. If you don't have streamlit installed then `pip install streamlit`
 3.  Go to the root directory of project and run `streamlit run -main.py` in the terminal . This will open an interactive web application. Now drag and drop and see the Magic
 <br>
 Happy Colorization :hugs: !! 
 
 ## References
 Paper: [Deep Koalarization: Image Colorization using CNNs and Inception-ResNet-v2 ](https://arxiv.org/pdf/1712.03400v1.pdf)
 
## License
All rights reserved under MIT License
