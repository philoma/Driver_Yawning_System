# Driver_Yawning
There are some rules and codes of conduct for those who drive irrespective of their social status. One of them is staying alert and active while driving.
Neglecting our duties towards safer travel has enabled hundreds of
thousands of tragedies to get associated with this wonderful invention
every year. It may seem like a trivial thing to most folks but following rules
and regulations on the road is of utmost importance.
So, <b>in order to mitigate the chances of road accidents, I've built an AI-ML model to alert the driver of his conciousness while driving the vehicle.<b>
  <br>
  System Model:
  <br>
![image](https://user-images.githubusercontent.com/87674698/160824721-4bf7b95b-fbc2-4961-a002-c62c92d74f3b.png)  <br>
  <h2>Implementation: </h2>
  1 --> In this program we used Dlib, a pre-trained program trained on the
HELEN dataset to detect human faces using the pre-defined 68
landmarks.
  
  ![image](https://user-images.githubusercontent.com/87674698/160772991-76839315-5781-4e13-9934-1366e7d28b68.png)
  
  2 -->  After passing our video feed to thedlib frame by frame, we are able to
detect left eye and right eye features of the face.
  
  3 --> Now, we drew contours around it using OpenCV.
  
  4 -->  Using Scipy’s Euclidean function, we calculated sum of both eyes’
aspect ratio which is the sum of 2 distinct vertical distances between
the eyelids divided by its horizontal distance.
  
 ![image](https://user-images.githubusercontent.com/87674698/160823758-564284fa-4ec2-478d-860b-d2b5a2ec604f.png)

  
  5-->  Now we check if the aspect ratio value is less than 0.25 (0.25was
chosen as a base case after some tests). If it is less the user is warned.

  <h1>Results: </h1>
  
  ![image](https://user-images.githubusercontent.com/87674698/163694998-876cbf42-9f16-428c-b4c0-78cd6aa98e44.png)

