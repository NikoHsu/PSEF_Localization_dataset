# PSEF_Localization: Point cloud and Senmatic map dataset in underground enviroment.


This is the dataset website for our paper **PSEF: Point Cloud and Semantic ESKF Fusion System For Precise and Robust Localization in Underground Parking Environments
**
Location and mapping data set of underground parking lot.

![nav](/demo/PSEF_demo.gif)


Two bag files, corresponding to the senmatic map and the point cloud map data under **normal conditions** and **full parking spaces**.


**Parameter setting**

#Installation angles of six cameras

rotateDeg0: 0

rotateDeg1: -1.0471975511965976

rotateDeg2: -2.0943951023931953

rotateDeg3: -3.141592653589793

rotateDeg4: 2.0943951023931953

rotateDeg5: 1.0471975511965976


        K: [337.2084410968044, 0.0, 320.5, 

        0.0, 337.2084410968044, 240.5, 
        
        0.0, 0.0, 1.0]

        
#Relative to the ground coordinate system

        R0: [0, 1.0, 0, 

        0.0, 0, 1, 
        
        1.0, 0.0, 0.0]
        
        T0: [0,

        1.23,
     
        0.0]


#LiDAR  VLP-16 16channels 10Hz

#IMU 200Hz noise  [0.01,0.01]

#camera 30Hz  size 640X480

#Camera external parameter
         lidar_to_imu:0,0,1,0.3,-1,0,0,1.5,-0,-1,-0,0,0,0,0,1;

 
         camera-to-imu:
         [0, 1.0, 0, 0,
 
        0.0, 0, 1, 1.0,
        
        1.0, 0.0, 0.0,0.0]

        
**Download link**

Because the file size of the data set is much larger than the file size limit of GitHub, the file is transferred to the cloud disk here, and the download address of URL is provided.

link:
https://pan.baidu.com/s/1GOsbk-sSezOEB634Uhx9rA 

Extraction code:
fjos

You can use tools provided by ROS, such as rosbag, to create, read and process bag files.
