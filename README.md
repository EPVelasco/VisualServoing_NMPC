# Visual Servoing + NMPC
This repository combines visual srvoing projected to a null space operator and Nonlinear Model Predictive Control (NMPC). The controller is used for autonomous navigation over photovoltaic arrays.

## Requirements 
We have tested this application on a DJI Matrice 100 drone with a Jetson Orin onboard computer. As image sensor we have an Intel Realsense D435i camera. In addition, it is necessary to have ROS Noetic and docker installed. 

To use our approach you need the [Visual Servoing](https://github.com/EPVelasco/vision_matrice100) and [NMPC](https://github.com/lfrecalde1/NMPC_Matrice_100) package. Also, it is necessary to run the algorithms of the NMPC package inside a [docker](https://github.com/EPVelasco/acados_casadi_ml_Jetson). This docker is optimized to use Acados and Casadi as NMPC solver for the Jetson Orin platform (ARM architecture). If you want to use the Acados and Casadi solver on an AMD architecture for experiments, you can use the [docker](https://github.com/EPVelasco/acados_casadi_ml) for AMD.


