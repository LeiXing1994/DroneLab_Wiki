## Simulation Task
#### 1. launch SITL  
 ```shell
 make posix_sitl_defaut gazebo
 ```

#### 2.launch mavros
```shell
roslaunch mavros px4.launch
```
#### 3.launch rqt
```shell
rqt
```
#### 4.open topics monitor, service caller and message publisher in plugins of rqt

#### 5.monitor drone through topics monitor
- ~/state
- ~/local_position/pose
- ~/setpoint_position/local
#### 6.send coordinate through message publisher
- ~/setpoint_position/local
#### 7.call service through service caller
- ~/set_mode
- Custom_mode=OFFBOARD
- ~/cmd/arming
- Value=TRUE
