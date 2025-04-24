# csci435-csci935-computer-vision-algorithms-and-systems-solved



**<span style='color:red'>TO GET THIS SOLUTION VISIT:</span>** https://www.ankitcodinghub.com/product/csci435-csci935-computer-vision-algorithms-and-systems-solved-2/

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;11288&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;4&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (4 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CSCI435\/CSCI935 Computer Vision: Algorithms and Systems Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">
            
<div class="kksr-stars">
    
<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
    
<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>
                

<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (4 votes)    </div>
    </div>
<h1>Assignment</h1>
<ul>
<li>Design a C (or C++) program that detects keypoints from an image and compare two images based on SIFT descriptors.</li>
<li>The assignment can be completed by either <strong>individuals</strong> or <strong>a group of two students</strong>.</li>
</ul>
<h1>Task</h1>
Recent research has revealed that keypoint-based descriptors are effective to characterize both individual objects and entire images. Such descriptors are widely used in object detection and image comparison. In this assignment, you are required to develop a program in C/C++ using OpenCV 3.4.1 to detect and display keypoints from an image and to compare two images based on SIFT descriptors.

The program should be able to take <strong>one</strong> or <strong>multiple image files</strong>. <em>When a single image file, e.g. </em>A.jpg<em>, is supplied to the program</em>, it should

<ol>
<li>Rescale the image to a size comparable to VGA size (480(rows) x 600(columns)) to reduce the computation. Note that the aspect ratio of the image should be kept when the image is rescaled.</li>
<li>Extract SIFT keypoints from the Y component of the image</li>
<li>For each detected keypoint, draw a <strong>cross</strong> “+” at the location of the key point and <strong>a circle</strong> around the keypoint whose radius is proportional to the scale of the keypoint.</li>
<li>Both the original image and the image with highlighted keypoints should be displayed in a window as follow</li>
</ol>
<table width="331">
<tbody>
<tr>
<td width="165"><strong>Original Image (rescaled)</strong></td>
<td width="165"><strong>Image with highlighted keypoints</strong></td>
</tr>
</tbody>
</table>
&nbsp;

<ol start="5">
<li>In the command window, the program should output the number of detected keypoints, e.g.</li>
</ol>
# of keypoints in A.jpg is <em>3180</em>

When multiple image files, say A.jpg, B.jpg, C.jpg, D.jpg and E.jpg, are supplied to the program as commend auguments, the program will compare each pair of the images using a Bag-of-Words model constructed from SIFT descriptors. Specifically, the program shall

<ol>
<li>Rescale all images to sizes comparable to VGA size (480×600) to reduce the computation. Note that the aspect ratio of the images should be kept when the image is rescaled, but there is no need to rescale all images to the same size.</li>
<li>Extract SIFT keypoints and descriptors from the Y-components of all scaled images.</li>
<li>Cluster the SIFT descriptors from ALL images into K-clusters using K-means algorithm. The values of K should be specified as a percentage of the total number of keypoints. Each cluster represents a visual word.</li>
<li>For each image, construct a histogram of the occurrence of the visual words. This should be done by classifying each SIFT descriptor of the image into one of the K-clusters (words) and continuing how many time each word occurred in the image.</li>
<li>For each pair of images, calculate the <sup>2</sup> distance between the histograms of the images. This <sup>2</sup> distance is a measurement of the <strong><em>dissimilarity</em></strong> of the pair of images.</li>
<li>The program should <strong>output</strong> the following information
<ol>
<li>Number of keypoints for each image and the total number of keypoints of all images, e.g.</li>
</ol>
</li>
</ol>
# of keypoints in A.jpg is 2138

# of keypoints in B.jpg is 923

# of keypoints in A.jpg is 780

# of keypoints in B.jpg is 1300

# of keypoints in A.jpg is 1578

&nbsp;

<ol>
<li>Dissimilarity matrices for K=5%, 10% and 20% of the total number of keypoints from all images. Note: please arrange the dissimilarity matrices in a readable format, e.g.</li>
</ol>
K=5%*(total number of keypoionts)=250

Dissimilarity Matrix

A &nbsp;&nbsp;&nbsp; B &nbsp;&nbsp;&nbsp; C &nbsp;&nbsp;&nbsp; D &nbsp;&nbsp;&nbsp; E

<ul>
<li>0 0.01 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 0.9</li>
<li>0</li>
<li>0</li>
<li>0 0.85</li>
<li>0</li>
</ul>
&nbsp;

K=10%*(total number of keypoionts)=500

Dissimilarity Matrix

A &nbsp;&nbsp;&nbsp; B &nbsp;&nbsp;&nbsp; C &nbsp;&nbsp;&nbsp; D &nbsp;&nbsp;&nbsp; E

<ul>
<li>0 0.01 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 0.9</li>
<li>0</li>
<li>0</li>
<li>0 0.85</li>
<li>0</li>
</ul>
&nbsp;

K=20%*(total number of keypoionts)=1000

Dissimilarity Matrix

A &nbsp;&nbsp;&nbsp; B &nbsp;&nbsp;&nbsp; C &nbsp;&nbsp;&nbsp; D &nbsp;&nbsp;&nbsp; E

<ul>
<li>0 0.01 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 0.9</li>
<li>0</li>
<li>0</li>
<li>0 0.85</li>
<li>0</li>
</ul>
&nbsp;

However, the program neither needs to display the original images nor the images with highlighted keypoints in this case.

Fifteen images covering different scenarios are provided for testing your program.

<h1>Requirements on coding</h1>
<ol>
<li>The program should be named as “<strong>siftImages</strong>” and shall take one or multiple image files as input, e.g. siftImages <em>imagefile1 [, imagefile2, imagefile3,…]</em>.</li>
<li>No other third-party libraries should be used in the program except OpenCV 3.4.1. The code has to be in C/C++.</li>
<li>The code should be modularized with detail comments AND all source code should be placed in a single file “cpp” or “siftImages.c”.</li>
</ol>
&nbsp;
