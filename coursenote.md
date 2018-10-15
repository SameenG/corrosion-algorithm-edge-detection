## lesson 1 （ img manipulation)

-  numpy(np) &  matplotlib.pyplot (plt) & scipy.ndimage(nd)
- structure of an img's numpy array : img [ pixel, pixel, channel ]  
#### founctions used
  - plt.imread/imshow/colorbar/plot/grid/legend/titlr/colorbar
  - img.cpoy /max/shape
  - np. zeros /histogram
  - nd.rotate / filters
 #### add
  - histogram :np.histograms returns left and right bin margins.
  ## lesson 2 (convolution and filtering)
  
  - np & nd & plt
  - convolve : f* h
  #### founctions
  - np.eye/ zeros_like /fft /real
  - nd.convolve
  
  #### add
  - 2d convolution
  - FFT  (http://blog.jobbole.com/70549/)
  - Remember that a convolution in **real space** is equivalent to a multiplication in **Fourier space** .

## lesson 3 （interpolation）

- np & plt & nd
- some concepts and basic interpretation: https://www.cambridgeincolour.com/tutorials/image-interpolation.htm


### founctions
- list slices::
- np.mean/ reshape/ 
- nd.convolve

### algorithms
> adaptive : some cannot be used to distort or rotate an image
> non-adaptive : nearest neighbor, bilinear, spline, sinc etc. The more adjecent pixels they include, the more accurate they can be.


