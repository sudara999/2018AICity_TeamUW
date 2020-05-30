## How to Use

1. Set the parameters in the configuration file if necessary. 
   1. The user needs to provide an approximate range (ideally 0.5 to 1 meter) of camera height in `calCamHeiMax` and `calCamHeiMin`.
   2. For manual calibration, if `calSelVanLnFlg` is not set, the user can manually input the 2D coordinates of two vanishing points Vr (on the right) and Vl (on the left) respectively in `calVr` and `calVl`. Otherwise, s/he can select two pairs of vanishing lines, i.e., parallel lines on the ground plane in 3D that are perpendicular to each other, in the window of “selector of vanishing lines”. Please select a pair of vanishing lines first and then another pair. There should be 8 points clicked in total. After the selection of vanishing lines is done, click `o`. Then, the window “3D grid on ground plane” will appear showing the update of calibration result. 
   3.	When `calEdaOptFlg` is set, the camera parameters will be optimized by the estimation of distribution algorithm (EDA) to minimize reprojection error. The user can input the end points of line segments and their true 3D distances respectively in `calMeasLnSegNdPt` and `calMeasLnSegDist`. 
   
2. Run the executable file.

```./bin```
