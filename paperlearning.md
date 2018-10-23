
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
### **《医学影像重建》**
#### chapter 1 tomograph
1. projection
2. image reconstruction (Filtered Backprojection)
3. Backprojection
4. mathematical expression
### chapter 2 
- Central slice theorem（Fourier Slice Theorem） 【https://blog.csdn.net/Terrenceyuu/article/details/65629938】
- reconstruct algorithm

---

### *Image reconstruction using simulated annealing in electrical impedance tomography: a new approach*
SA approach
#### 1.introduction
- difference methods and absolute methods
> difference: two electrical potential data-sets are measured corresponding to two different conductivity distributions 
> absolute : single data-set / the aim is to estimate the absolute conductivity distribution  *solve the ill-posed,inverse problem*

- fwd and inverse problem
> fwd : FDM

> inverse : minimizes the difference between measured and calculated potentials by the forward problem *requires a competent regularization/optimization method * 

### **generic algorithm and simulated annealing method(SA)**
- The choice of the **cooling rate** and **the new candidate solution** are the most important decisions in a SA algorithm

### 2. fwd problem
- model the potential:  **∇ (σ∇u) =0**
- boundary condition(BC) : Neumann BC (know the derivative) and Dirichlet BC(potential at the boundary is known) 
[ ] **detail calculation remain to be read**

### 3. inverse problem
> inverse problems are formulated as optimization problems with constraints given by: square(min(A(u) − f)) where A(u) is the forward problem solution and f are empirical data.__Tikhonov regularization__ is commonly added. Other regularized methods are mentioned.

### 4. SA
- new distributions must be sought randomly and then find the one that **decrease the objective function value** (increasing one can be accepted depending on P __Metropolis criterion__ )

#### 4.1 old sa approach
- impose restrictions to get new candidate points (computationally expensive: step matrix(different directions) , fwd problems)

### proposed sa approach
- define a step delta = Dmxn* alpha
- regularization:low-pass Gaussian filter to smooth the Dmxn
> __expression: σ(k+1)= σ(k)+ α((LDmxn) ◦ σ(k))__
> modified stepsize and parameters used for it
 
### procedure :initialize(parameters)--> σ(k+1)-->accept the σ(k+1) matrix or not according to SA -->iteration

### problems and disscussions

