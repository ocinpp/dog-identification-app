# Dog Identification App

Using CNN and transfer learning to build a dog classification app as a project for Udacity

## Libraries

8 python libraries are required

- keras
- sklearn
- numpy
- pandas
- glob
- cv2
- matplotlib
- tqdm

If they are not yet installed, you can use pip to install

## Data

These bottleneck feature files have to be downloaded to the directory **bottleneck_features**

- [VGG-19 bottleneck features](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/DogVGG16Data.npz)
- [Inception bottleneck features](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/DogInceptionV3Data.npz)

## Running the app

Put the image in the directory **my_test_images** and pass the path to the function *my_predictor*. The prediction will then be returned. If the source image does not resember a human face or a dog, the message *"Error. Not a face or a dog detected in the image"* will be returned.

```python
res = my_predictor('my_test_images/dog_test1.jpg')
print(res)
```
