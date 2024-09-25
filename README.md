# VideoRun2D

***
# About
We present VideoRun2D, a new markerless biomechanic sprint analysis system based on deep learning models. This system was initially described technically and scientifically in this [arXiv technical report](https://arxiv.org/abs/2409.10175) and published after peer review at the [IAPR](https://iapr.org/)  Intl. Conf. on Pattern Recognition ([ICPR](https://icpr2024.org/)), Kolkata, India, December 2024. (2<sup>nd</sup> Workshop on Facial and Body Expressions, [FBE](https://sites.google.com/unifi.it/fbe2024/)) [[PDF](https://arxiv.org/abs/2409.10175)].

Our proposed VideoRun2D performs markerless body tracking and estimates multiples joint angles across time during a sprint. To achieve effective estimation, the VideoRun2D system comprises five processing modules: video pre-processing, tracking of the articular points, tracking post-processing, biomechanical features generation, and a validation system that employs statistical analysis. 

![1](./media/Diagrama.png)



https://github.com/user-attachments/assets/6073b6d5-8905-451d-b9da-5a1031fa604c



https://github.com/user-attachments/assets/3d526f81-b182-47d2-982c-ee193845b8b3



# Motivation

Sprinting is a determinant ability, especially in team sports. The kinematics of the sprint have been studied in the past using different methods specially developed considering human biomechanics and, among those methods, markerless systems stand out as very cost-effective. On the other hand, we have now multiple general methods for pixel and body tracking based on recent machine learning breakthroughs with excellent performance in body tracking, but these excellent trackers do not generally consider realistic human biomechanics (like the ones considered in support for professional sports or injury rehabilitation). This investigation first adapts two of these general trackers (MoveNet and CoTracker) for realistic biomechanical analysis and then evaluates them in comparison to manual tracking based on manually-marked key points (Kinovea). 


# Database

## Data acquisition

Five healthy amateur soccer players are analyzed (23±3.74 years old, 77.2±6.8 kg weight, 181.8±6.3 cm height). All of them signed an informed consent. The investigation was approved by the Ethics Committee of the University following the Declaration of Helsinki.

The sprints were recorded using a video camera Panasonic DMC FZ-1000 with a resolution of 1920x1080p and recorded at 100 fps in two different outdoor scenarios. Each subject performed eight sprints of 20m while the camera recorded between the 5th and 15th m. The camera was placed 10 m from the middle point of the sprint. All the players sprinted with football boots on a natural grass field. Between each sprint, the players had 5 minutes of rest. A total of 40 sprints and 240 running strides were generated.

## Ground truth based on manual labeling (Kinovea)

Three experts previously trained manually marked all the images using the freeware Kinovea (version 0.9.5); and these marks are used as ground truth. The main instruction given to the experts was to mark the different points on the joint centers (shoulder, hip, knee, and ankle).

![2](./media/JointPoints.png)

For the body parts covered by other segments, the experts were instructed to mark the anatomical points as if the different body parts covering others were transparent. These points were marked in every frame of each video. When all the frames were labeled, the trajectory of each joint was revised to find and correct possible marking mistakes.

# Instructions for downloading the VideoRun2D dataset

Under construction


# Publications

+ G. Garrido-Lopez, L.F. Gomez, J. Fierrez, A. Morales, R. Tolosana, J. Rueda, and E. Navarro, "VideoRun2D: Cost-Effective Markerless Motion Capture for Sprint Biomechanics", in Proc. IAPR Intl. Conf. of Pattern Recognition Worshops (ICPRw), Kolkata, India, December 2024. [[PDF](https://arxiv.org/pdf/2409.10175)]

# Contact:

For more information contact Profs. Julian Fierrez and Enrique Navarro: julian.fierrez@uam.es and enrique.navarro@upm.es

