ABSTRACT 
The face is one of the easiest ways to distinguish the individual identity of each other. Face recognition is a personal identification system that uses personal characteristics of a person to identify the person's identity. Human face recognition procedure basically consists of two phases, namely face detection, where this process takes place very rapidly in humans, except under conditions where the object is located at a short distance away, the next is the introduction, which recognize a face as individuals. Stage is then replicated and developed as a model for facial image recognition (face recognition) is one of the much-studied biometrics technology and developed by experts. There are two kinds of methods that are currently popular in developed face recognition pattern namely, Eigenface method and Fisher face method. Facial image recognition Eigenface method is based on the reduction of face dimensional space using Principal Component Analysis (PCA) for facial features. The main purpose of the use of PCA on face recognition using Eigen faces was formed (face space) by finding the eigenvector corresponding to the largest eigenvalue of the face image. The area of this project face detection system with face recognition is Image processing. The software requirements for this project are MATLAB software. 
Keywords: face detection, Eigen face, PCA, MATLAB
Extension: There are vast number of applications from this face detection project, this project can be extended that the various parts in the face can be detect which are in various directions.

INTRODUCTION

Face recognition is the task of identifying an already detected object as a known or unknown face. Often the problem of face recognition is confused with the problem of face detection Face Recognition on the other hand is to decide if the "face" is someone known, or unknown, using for this purpose   a database of faces in   order to validate this input face. 
 

FACE RECOGNIZATION:

DIFFERENT APPROACHES OF FACE RECOGNITION:
There are two predominant approaches to the face recognition problem:  Geometric (feature based) and photometric (view based).  As researcher interest in face recognition continued, many different algorithms were developed, three of which have been well studied in face recognition literature.   
Recognition algorithms can be divided into two main approaches:   
1.	Geometric : Is based on geometrical relationship between facial landmarks, or in other words the spatial configuration of facial features. That means that the main geometrical features of the face such as the eyes, nose and mouth are first located and then faces are classified on the basis of various geometrical distances and angles between features.  (Figure 3) 
2.	Photometric Stereo: Used to recover the shape of an object from a number of images taken under different lighting conditions.  The shape of the recovered object is defined by a gradient map, which is made up of an array of surface normal (Zhao and Chalupa, 2006) (Figure 2)  
Popular recognition algorithms include:
1.	Principal Component   Analysis using Eigenfaces, (PCA)   
2.	Linear   Discriminate Analysis,   
3.	Elastic Bunch Graph Matching using the Fisher face   algorithm

  

FACE DETECTION:
Face detection involves separating image windows into two classes; one containing faces (turning the background (clutter). It is difficult because although commonalities exist between faces, they can vary considerably in terms of age, skin color and facial expression. The problem is further complicated by differing lighting conditions, image qualities and geometries, as well as the possibility of partial occlusion and disguise. An ideal face detector would therefore be able to detect the presence of any face under any set of lighting conditions, upon any background. The face detection task can be broken down into two steps. The first step is a classification task that takes some arbitrary image as input and outputs a binary value of yes or no, indicating whether there are any faces present in the image. The second step is the face localization task that aims to take an image as input and output the location of any face or faces within that image as some bounding box with (x, y, width, height). 
The face detection system can be divided into the following steps: -
1.	Pre-Processing: To reduce the variability in the faces, the images are processed before they are fed into the network. All positive examples that is the face images are obtained by cropping images with frontal faces to include only the front view. All the cropped images are then corrected for lighting through standard algorithms. 
2.	Classification: Neural networks are implemented to classify the images as faces or nonfaces by training on these examples. We use both our implementation of the neural network and the MATLAB neural network toolbox for this task. Different network configurations are experimented with to optimize the results.  
3.	Localization: The trained neural network is then used to search for faces in an image and if present localize them in a bounding box. Various Feature of Face on which the work has done on: - Position Scale Orientation Illumination 



 

LITERATURE SURVEY
Face detection is a computer technology that determines the location and size of human face in arbitrary (digital) image. The facial features are detected and any other objects like trees, buildings and bodies etc. are ignored from the digital image. It can be regarded as a ‗specific ‘case of object-class detection, where the task is finding the location and sizes of all objects in an image that belong to a given class. Face detection, can be regarded as a more ‗general ‘case of face localization. In face localization, the task is to find the locations and sizes of a known number of faces (usually one). Basically, there are two types of approaches to detect facial part in the given image i.e., feature base and image base approach. Feature base approach tries to extract features of the image and match it against the knowledge of the face features. While image base approach tries to get best match between training and testing images. 
 
Fig 2.1 detection methods 

FEATURE BASE APPROCH: 
Active Shape Model Active shape models focus on complex non-rigid features like actual physical and higher-level appearance of features Means that Active Shape Models (ASMs) are aimed at automatically locating landmark points that define the shape of any statistically modelled object in an image. When of facial features such as the eyes, lips, nose, mouth and eyebrows. The training stage of an ASM involves the building of a statistical 
a)	facial model from a training set containing images with manually annotated landmarks. 
ASMs is classified into three groups i.e., snakes, PDM, Deformable templates  
b)	1.1) Snakes: The first type uses a generic active contour called snakes, first introduced by Kiss et al. in 1987 Snakes are used to identify head boundaries [8,9,10,11,12]. In order to achieve the task, a snake is first initialized at the proximity around a head boundary. It then locks onto nearby edges and subsequently assume the shape of the head. The evolution of a snake is achieved by minimizing an energy function, Snake (analogy with physical systems), denoted as snake = Internal + ExternalWhere internal and External are internal and external energy functions. Internal energy is the part that depends on the intrinsic properties of the snake and defines its natural evolution. The typical natural evolution in snakes is shrinking or expanding. The external energy counteracts the internal energy and enables the contours to deviate from the natural evolution and eventually assume the shape of nearby features—the head boundary at a state of equilibria. Two main considerations for forming snakes i.e., selection of energy terms and energy minimization. Elastic energy is used commonly as internal energy. Internal energy is varied with the distance between control points on the snake, through which we get contour an elastic-band characteristic that causes it to shrink or expand. On other side external energy relay on image features. Energy minimization process is done by optimization techniques such as the steepest gradient descent. Which needs highest computations. Huang and Chen and Lam and Yan both employ fast iteration methods by greedy algorithms. Snakes have some demerits like contour often becomes trapped onto false image features and another one is that snakes are not suitable in extracting non convex features. 


  FEATURE ANALYSIS 
These algorithms aim to find structural features that exist even when the pose, viewpoint, or lighting conditions vary, and then use these to locate faces. These methods are designed mainly for face localization 
Feature Searching 

Paul Viola and Michael Jones presented an approach for object detection which minimizes computation time while achieving high detection accuracy. Paul Viola and Michael Jones [39] proposed a fast and robust method for face detection which is 15 times quicker than any technique at the time of release with 95% accuracy at around 17 fps. The technique relies on the use of simple Har-like features that are evaluated quickly through the use of a new image representation. Based on the concept of an ―Integral Image‖ it generates a large set of features and uses the boosting algorithm AdaBoost to reduce the overcomplete set and the introduction of a degenerative tree of the boosted classifiers provides for robust and fast interferences. The detector is applied in a scanning fashion and used on gray-scale images, the scanned window that is applied can also be scaled, as well as the features evaluated. 

CONSTELLATION METHOD 
All methods discussed so far are able to track faces but still some issue like locating faces of various poses in complex background is truly difficult. To reduce this difficulty investigator, form a group of facial features in face-like constellations using more robust modelling approaches such as statistical analysis. Various types of face constellations have been proposed by Burl et al. They establish use of statistical shape theory on the features detected from a multiscale Gaussian derivative filter. Huang et al. also apply a Gaussian filter for pre-processing in a framework based on image feature analysis. Image Base Approach. 


DIGITAL IMAGE PROCESSING
DIGITAL IMAGE PROCESSING 
Interest in digital image processing methods stems from two principal application areas:
1.	Improvement of pictorial information for human interpretation 
2.	Processing of scene data for autonomous machine perception 
In this second application area, interest focuses on procedures for extracting image information in a form suitable for computer processing. 
Examples includes automatic character recognition, industrial machine vision for product assembly and inspection, military recognizance, automatic processing of fingerprints etc. 
Image: 
Am image referring a 2D light intensity function f (x, y), where (x, y) denotes spatial coordinates and the value of f at any point (x, y) is proportional to the brightness or gray levels of the image at that point. A digital image is an image f (x, y) that has been discretized both in spatial coordinates and brightness. The elements of such a digital array are called image elements or pixels.
A simple image model: 
To be suitable for computer processing, an image f (x, y) must be digitalized both spatially and in amplitude. Digitization of the spatial coordinates (x, y) is called image sampling. Amplitude digitization is called   gray-level quantization.
The storage and processing requirements increase rapidly with the spatial resolution and the number of gray levels. 
Example: A 256 gray-level image of size 256x256 occupies 64k bytes of memory. 
      Types of image processing
•	Low level processing 
•	Medium level processing 
•	High level processing 
Low level processing means performing basic operations on images such as reading an image resize, resize, image rotate, RGB to gray level conversion, histogram equalization etc…, The output image obtained after low level processing is raw image. Medium level processing means extracting regions of interest from output of low-level processed image. Medium level processing deals with identification of boundaries i.e.,edges. This process is called segmentation. High level processing deals with adding of artificial intelligence to medium level processed signal. 
 FUNDAMENTAL STEPS IN IMAGE PROCESSING 
Fundamental steps in image processing are 
1.	Image acquisition: to acquire a digital image 
2.	Image pre-processing: to improve the image in ways that increases the chances for success of the other processes. 
3.	Image segmentation: to partitions an input image into its constituent parts of objects. 
4.	Image segmentation: to convert the input data to a from suitable for computer processing. 
5.	Image description: to extract the features that result in some quantitative information of interest of features that are basic for differentiating one class of objects from another. 
6.	Image recognition: to assign a label to an object based on the information provided by its description. 
 
fig.3.1. Fundamental steps in digital image processing  
ELEMENTS OF DIGITAL IMAGE PROCESSING SYSTEMS
A digital image processing system contains the following blocks as shown in the figure 
 
                             Fig.3.3. Elements of digital image processing systems   
The basic operations performed in a digital image processing system include 
1.	Acquisition 
2.	Storage 
3.	Processing 
4.	Communication 
5.	Display 
A simple image formation model
Image is denoted by two-dimensional function f (x, y). f (x, y) may be characterized by 2 components: 
1.	The amount of source illumination I (x, y) incident on the scene 
2.	The amount of illumination reflected r (x, y) by the objects of the scene 
3.	f (x, y) = I (x, y) r (x, y), where 0 <I(XXY) <and 0<r (x, y) < 1 


Typical values of reflectance r (x, y):
•	0.01 for black velvet 
•	0.65 for stainless steel 
•	0.8 for flat white wall paint 
•	0.9 for silver-plated metal 
•	0.93 for snow Example of typical ranges of illumination I (x, y) for visible light 
(Average values)                                                                                                                             
•	Sun on a clear day: ~90,000 lm/m^2, down to 10,000lm/m^2 on a cloudy day 
•	Full moon on a clear evening: -0.1 lm/m^2 
•	Typical illumination level in a commercial office. ~1000lm/m^2 image Formats (supported by MATLAB Image Processing Toolbox)  
Format name   	Full name  	Description 	Recognized extensions  
TIFF 	Tagged Image File 
Format 	A flexible file format supporting a variety image compression standard including 
JPEG 	.tiff, .tiff 
JPEG 	Joint Photographic 
Experts Group  	A standard for compression of images of photographic quality 	.jpg, .jpeg 
GIF 	Graphics 
Interchange Format 	Frequently used to make small animations 
on the internet 	.gif 
BMP 	Windows Bitmap  	Format used mainly for simple uncompressed images 	.bmp 
PNG 	Portable 	Network 
Graphics  	Compresses full color images with transparency (up to 
48bits/p 	. pang
                                   Table.3.3. Image Formats Supported By MATLAB 



FACE DETECTION 
The problem of face recognition is all about face detection. This is a fact that seems quite bizarre to new researchers in this area. However, before face recognition is possible, one must be able to reliably find a face and its landmarks. This is essentially a segmentation problem and in practical systems, most of the effort goes into solving this task. In fact, the actual recognition based on features extracted from these facial landmarks is only a minor last step.
There are two types of face detection problems:
1)	Face detection in images and 
2)	Real-time face detection 
FACE DETECTION IN IMAGES
 
            Figure 5.1 A successful face detection in an image with a frontal view of a human face.
Most face detection systems attempt to extract a fraction of the whole face, thereby eliminating most of the background and other areas of an individual's head such as hair that are not necessary for the face recognition task. With static images, this is often done by running a across the image. The face detection system then judges if a face is present inside the window (Brunelle and Poggi, 1993). Unfortunately, with static images there is a very large search space of possible locations of a face in an image 
Most face detection systems use an example-based learning approach to decide whether or not a face is present in the window at that given instant (Sung and Poggio,1994 and sung,1995). A neural network or some other classifier is trained using supervised learning with 'face' and 'nonface' examples, thereby enabling it to classify an image (window in face detection system) as a 'face' or 'non-face’. Unfortunately, while it is relatively easy to find face examples, how would one find a representative sample of images which represent non-faces (Rowley et al., 1996)? Therefore, face detection systems using example-based learning need thousands of 'faces' and 'nonface' images for effective training. Rowley, Baluga, and Kaneda (Rowley et al.,1996) used 1025 face images and 8000 non-face images (generated from 146,212,178 sub-images) for their training set!
There is another technique for determining whether there is a face inside the face detection system's window - using Template Matching. The difference between a fixed target pattern (face) and the window is computed and thresholder. If the window contains a pattern which is close to the target pattern(face) then the window is judged as containing a face. An implementation of template matching called Correlation Templates uses a whole bank of fixed sized templates to detect facial features in an image (Bichsel, 1991 &Brunelle and Poggi, 1993). By using several templates of different (fixed) sizes, faces of different scales (sizes) are detected. The other implementation of template matching is using a deformable template (Yuille, 1992). Instead of using several fixed size templates, we use a deformable template (which is non-rigid) and there by change the size of the template hoping to detect a face in an image.
A face detection scheme that is related to template matching is image invariants. Here the fact that the local ordinal structure of brightness distribution of a face remains largely unchanged under different illumination conditions (Sinha, 1994) is used to construct a spatial template of the face which closely corresponds to facial features. In other words, the average grey-scale intensities in human faces are used as a basis for face detection. For example, almost always an individual’s eye region is darker than his forehead or nose. Therefore, an image will match the template if it satisfies the 'darker than' and 'brighter than' relationships (Sung and Poggi, 1994).
REAL-TIME FACE DETECTION
Real-time face detection involves detection of a face from a series of frames from a video capturing device. While the hardware requirements for such a system are far more stringent, from a computer vision stand point, real-time face detection is actually a far simpler process than detecting a face in a static image. This is because unlike most of our surrounding environment, people are continually moving. We walk around, blink, fidget, wave our hands about, etc.
