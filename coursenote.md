## lesson 1 （ img manipulation)

-  numpy(np) &  matplotlib.pyplot (plt) & scipy.ndimage(nd)
- structure of an img's numpy array : img [ pixel, pixel, channel ]  
#### functions used
  - plt.imread/imshow/colorbar/plot/grid/legend/titlr/colorbar
  - img.cpoy /max/shape
  - np. zeros /histogram
  - nd.rotate / filters
 #### add
  - histogram :np.histograms returns left and right bin margins.
  ## lesson 2 (convolution and filtering)
  
  - np & nd & plt
  - convolve : f* h
  #### functions
  - np.eye/ zeros_like /fft /real
  - nd.convolve
  
  #### add
  - 2d convolution
  - FFT  (http://blog.jobbole.com/70549/)
  - Remember that a convolution in **real space** is equivalent to a multiplication in **Fourier space** .

## lesson 3 （interpolation）

- np & plt & nd
- some concepts and basic interpretation: https://www.cambridgeincolour.com/tutorials/image-interpolation.htm


### functions
- list slices::
- np.mean/ reshape/ 
- nd.convolve/.interpolation.rotate

### algorithms
> adaptive : some cannot be used to distort or rotate an image

> non-adaptive : nearest neighbor, bilinear, spline, sinc etc. The more adjecent pixels they include, the more accurate they can be.

## lesson 4 (segmentation)

### functions
- nd.label(label features in an array)/binary_opening(noise reduction)/closing(remove inner dots)/find_objects
- use of plt.imshow()/plt.hist
- image.astype()

## lesson 5(wave propagation) 

### points
> wave propagation :https://en.wikipedia.org/wiki/Wave_propagation

>sum along axis:https://stackoverrun.com/cn/q/11483910

### functions
np.angle
