# Old Photo Restoration Using Pix2Pix gan
This project uses PatchGAN, a popular generative adversarial network (GAN) architecture, to restore old images. PatchGAN is a type of discriminator that evaluates patches of an image instead of the entire image. This makes it well-suited for image restoration tasks, as it can focus on the local details of an image that are often lost in old photos.

The project first trains a PatchGAN discriminator on a dataset of real and fake images. The discriminator is then used to train a generator network that can produce realistic images that fool the discriminator. Once the generator is trained, it can be used to restore old images.

The project has been tested on a variety of old images, and it has been shown to be able to significantly improve the quality of the images. The restored images are sharper, more colorful, and have less noise than the original images.

Additionally, I tried image inpainting with the same architeure on similar dataset.

**Dataset:**

The project uses the Flickr-Faces-HQ Dataset (FFHQ) -Small. This dataset contains 3143 high-quality images of faces.It is a subset of orignal Flickr-Faces-HQ dataset. The images are split into a training set and validation set with ratio 90:10.

**Architecture**

![image](https://github.com/bimarshak7/GAN-image-restore/assets/59700049/44432487-4041-4147-8eb0-e64fd71b1627)


You can use Inference notebook to test and play with the model. Click the badge below.  
<a href="https://colab.research.google.com/github/bimarshak7/GAN-image-restore/blob/main/ImageRestoration_Model_Inference.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>

**Sample Input/Output**
![image](https://github.com/bimarshak7/GAN-image-restore/assets/59700049/1e18576a-23d7-4922-9562-40020dcf668b)

