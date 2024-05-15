# Avataar_Assignment
This repository contains the code file and the demonstration of using the code along with a demo result.

The process to run the code file is very simple - THe code is well documented.
1. Download the Avataar_Assignment.ipynb file
2. Change the path for the input point cloud as it suits you.

The methodology is very simple -  
1. Instead of using all heavy Deep Learning based solutions to segment the floor, I used a basic Open3D function and tested it on the given data which turned out to be good enough.
2. For the next deliverable, the process was simple as to compute a rotation matrix which would align the point cloud to the YZ plane.
3. This rotation could not be [ 1   0   0 ] becuase we dont know if the point cloud is always aligned to the XZ plane or not.
                              [ 0   0  -1 ]
                              [ 0   1   0 ]
4. So to find a rotation matrix, the series of steps are mentioned in the comments in the code file.

Better Approaches - 
1. We could Deep Learning approaches to create a mesh from the point cloud.
2. We could Deep Learning approaches to segment the point cloud but they will increase the inference time.
3. <img width="689" alt="pillow_both_snapshot01" src="https://github.com/saatvikmah/Avataar_Assignment/assets/77113517/5549819d-8d73-4f74-89f1-57d4bf0d40b9">
<img width="689" alt="pillow_snapshot00" src="https://github.com/saatvikmah/Avataar_Assignment/assets/77113517/d771f4a0-30c8-4dfc-a7af-90247b656a34">
