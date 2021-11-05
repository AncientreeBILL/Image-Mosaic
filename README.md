# Image-Mosaic
* This is a little project to reconstruct a color image with a set of images. 
* In the example notebook, I used [cifar-10][cifar] as the dataset. You can use your own images.
* The underlying theory is to replace the pixel patches with the images from the dataset who possess the closest color intensities.
* The process is a bit long, since the number of data is huge. So I add a dummy print string indication to show the progress. (I am considering using memoization tricks to save some already calculated results, therefore when facing the same pixel values again, the algorithm will directly pick up the most similar image patch rather than iterating the whole dataset again).

###  The example result is below. You can adjust the size of patches to be replaced.
* Input image:
![Input image](https://github.com/AncientreeBILL/Image-Mosaic/blob/main/test.JPG)

---

* Output image:
![Output image](https://github.com/AncientreeBILL/Image-Mosaic/blob/main/output.png)

### Have Fun!

[cifar]: https://www.cs.toronto.edu/~kriz/cifar.html
