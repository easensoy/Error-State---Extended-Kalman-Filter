# Error-State---Extended-Kalman-Filter

This project is all about implementation of an EKF for sensor fusion and estimation, using IMU, GNSS, and LIDAR measurements to estimate the vehicle's position, velocity, and orientation. The EKF combines the measurements with a motion model to provide accurate and consistent estimates of the vehicle's state.

## Phase 1: Fair Filter Test
In this phase, a fair filter test is conducted using the "pt1_data.pkl" file. The filter relies on IMU data to propagate the state forward in time, and GPS and LIDAR position updates to correct the state estimate. The purpose of this phase is to assess the performance of the filter in terms of state estimation accuracy and reliability when using these sensor inputs.

![phase1_1](https://github.com/easensoy/Error-State---Extended-Kalman-Filter/assets/76905667/3f0b801d-a840-469d-892c-0252fb28b78c)

![phase1_2](https://github.com/easensoy/Error-State---Extended-Kalman-Filter/assets/76905667/cda742b9-5e14-4288-a4ab-ec7bb4ffee15)


## Phase 2: Sensor Miscalibration Effects
In this phase, the effects of sensor miscalibration are examined. Specifically, the incorrect transformation between the LIDAR and the IMU sensor frame introduces errors in the vehicle pose estimates. The goal of this phase is to determine how to adjust the filter parameters, specifically the noise variances, to compensate for these errors. The "pt1_data.pkl" file is used for this analysis.

![phase2_1](https://github.com/easensoy/Error-State---Extended-Kalman-Filter/assets/76905667/9729721d-a89c-44dc-99a3-b1e37a5df145)

![phase2_2](https://github.com/easensoy/Error-State---Extended-Kalman-Filter/assets/76905667/8d38d652-f029-44dc-81f3-515ed13801e2)


## Phase 3: Sensor Dropout Effects
In this phase, the effects of sensor dropout are explored. Sensor dropout refers to a situation where all external positioning information from GPS and LIDAR is temporarily lost. The aim of this phase is to assess how the filter behaves and the performance of the state estimation during these periods of sensor dropout. The "pt3_data.pkl" file is utilized for this investigation.

![phase3_1](https://github.com/easensoy/Error-State---Extended-Kalman-Filter/assets/76905667/181d8be3-0fc7-4348-970e-dc9e7fa0af64)

![phase3_2](https://github.com/easensoy/Error-State---Extended-Kalman-Filter/assets/76905667/64cabcd7-6802-4cb7-be57-e8c2f8636154)


