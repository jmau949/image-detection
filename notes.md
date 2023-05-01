sagemaker studio = online ide
launch studio from domain
exclamation points means terminal commands
use this command to download a dataset
    * !kaggle datasets download -d paultimothymooney/chest-xray-pneumonia --force
    * https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia being the dataset

pretrained models can use only a fixed 224 x 224 image size.
pretrained meaning we will be using transfer learning, more specifically, resnet, built in image classifier

matplotlib saves or opens image in default colormap viridis
Pillow is the friendly PIL fork. PIL is the Python Imaging Library 
    * png image have have 'R', 'G', 'B' and 'A' band
    * RGBA have 4 dimensions unlike RGB which has 3 dimension
    * last dimension = Alpha, controls opacity of image

for car model detection
    * have to convert images to RGB to use pretrained models
    * to convert, use below code
        import PIL.Image

        rgba_image=PIL.Image.open('your_path')
        rgb_image = rgba_image.convert('RGB')


