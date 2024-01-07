# FiRaindrop
To fill the huge gaps in Single Image Deraining (SID) and promote related research on fisheye image processing, we propose a large-scale dataset named FiRaindrop for fisheye image deraining for the first time. 

## Description of FiRaindrop Dataset
FiRaindrop contains ~13.6K rain/rain-free fisheye image pairs and ~28K real rain images, covering more than 500 real-world scenes with different illumination and semantics. All these images are captured with two wide-angle lens cameras with resolutions of $1280 \times 720$.  The cameras are produced and used by an automobile manufacturer and their mode number is 51CAMZI03015. As shown in the left part of the Figure below, two wide-angle lenses are fixed to the rear of a vehicle using a simple bracket mold, so that we can easily keep the extrinsic of the cameras unchanged and conveniently take photos of different scenes. When taking rain/rain-free image pairs of a scene, we first keep the vehicle stationary and take pictures with a clean camera lens to get clean images. Then, we lightly sprayed the camera lens with a sprinkling to get light rain images. Finally, we sprinkled more water onto the lens to obtain heavy rain images. Each camera can get two image pairs i.e. light-rain/rain-free image pair and heavy-rain/rain-free image pair. Besides, we also take more than $\sim$28K additional images on rainy days without the rain-free (ground truth) images for subjective deraining evaluation. Compared with the real raindrop images, our synthesized raindrop image pairs have similar rain noise representation and distribution with pixel-aligned. 
![Fig-02](https://github.com/IntelligentDrivingCoding/FiRaindrop/assets/149981625/e2522ce3-1419-4926-9d3b-d23dc5e7280e)
![Fig-04-02](https://github.com/IntelligentDrivingCoding/FiRaindrop/assets/149981625/f5bfe72f-d026-4dd4-9955-8f995652cf90)
All these images are captured at hundreds of locations in Wuhan city in China throughout the day and night. To include scenes with moving objects and keep the pixels of image pairs aligned, we post-process each image pair by manually masking the misaligned part in both rain/rain-free images with black rectangles. For example, moving objects in the black circle regions in the last two rows in the Figure above will introduce misalignment for supervised deraining, so we remove those regions by masks (black circles drawn in the images) in both rain and rain-free images. At last,  we randomly select 9,350 image pairs from the entire dataset as the training set and 1,390 and 2,880 images as the eval and test set respectively. Real rainy images mentioned above are used as the real-world evaluation set. Quantitative comparisons are made on the eval and test set and qualitative comparison experiments are performed on the real-world 
evaluation set.



## Contactor

Wenqian Zhu, Email: zwq_pi@whu.edu.cn

To encourage related research, we will provide the dataset according to your request. Please email your full name and affiliation to the contact person (zwq_pi at whu dot edu dot cn). We ask for your information only to make sure the dataset is used for non-commercial purposes. We will not give it to any third party or publish it publicly anywhere. Due to the privacy issue we will not provide the license plates in the future. If you download our dataset, it means you have agreed to our terms of access in the email.

We currently make parts of the FiRaindrop dataset available, and the link is https://pan.baidu.com/s/1RK8E7eZxTl51LFAaPKNyUQ?pwd=f99v
