# swarm_control_stack_1
A selection of ros packages required to run boids swarming algorithms on Tito Neri vessels.

Requirements:
- Benchmark Tito Neri vessel with ros2 on the main computer (tested on ROS Iron)
- Environment variable VESSEL_ID set appropiately (e.g. RAS_TN_DB, RAS_TN_GR ...)

## Setup
Pull the content to the ros workspace
```
cd ~/ros2_ws/src/
```

```
git clone https://github.com/RAS-Delft/swarm_control_stack_1
```

```
git submodule update --init --recursive
```

Build
```
cd ~/ros2_ws; colcon build; source install/setup.bash
```


## Option 1: Run with simulator in the loop
```
ros2 launch boat_controller single_boid.launch.py
```

## Option 2: Run with ships in the loop
```
ros2 launch boat_controller single_boid.launch.py
```