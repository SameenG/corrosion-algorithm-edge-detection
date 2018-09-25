
### *deep learning-Guided Image Recongstruction from Incomplete Data* ( improve quality of image reconstruction )

#### related work
- CNN as a quasi-projection operator with least squares minimization 

- structure：similar to teh pro ximal gradient descent method which alternates between taking a step along the gradient of some cost function and applying a proximal operator

- an ill-posed inverse problem, a regulized sulotion needed


#### image reconstruction problem

- image objects decomposed into 2 parts, null space and orthogonal component


 *ref ：
 1.Non-iterative reconstruction of images from compressively sensed random measurements.
 2.Ashish Bora, Ajil Jalal, Eric Price, and Alexandros G Dimakis. Compressed sensing using generative models. arXiv preprint
 * 
 
 
 #### approach
 - replace P in traditional  proximal gradient descent by a quasi-projection operator Q(f,w)
 -
 
 ---
 
 - [x] FEM in EIT https://blog.csdn.net/baidu_38127162/article/details/75207769
 - [ ] forward/inverse problem in eit
 - [X] CNN
         
                 http://cs231n.github.io/convolutional-networks/
                 https://blog.csdn.net/v_july_v/article/details/51812459
                 *Zeiler, M. D., & Fergus, R. (2014, September). Visualizing and understanding convolutional networks.*

 
 
 - [ ] regularization https://en.wikipedia.org/wiki/Regularization_(mathematics)#Generalization
  - usage : applies to objective functions in ill-posed optimization problems. in classification,
  - some conceptions: 
  1. loss function: loss functions representing the price paid for inaccuracy of predictions in classification problems
  2. hinge loss:https://en.wikipedia.org/wiki/Hinge_loss 
 - regularization term R(f) is usually added to a loss founction,typically chosen to impose a penalty on the complexity of f.
   - Tikhonov regularization
   - Total variation regularization
 - [ ] proximal gradient descent
   - www.cs.cmu.edu/~pradeepr/convexopt/Lecture_Slides/prox-grad_2.pdf
