# Hospitalbot-Path-Planning-RL

### Prerequisites
```bash
cd gazebo-classic_plugins/attachmodel
cmake ..
make
sudo cp -r libAttachModelPlugin.so /usr/lib/x86_64-linux-gnu/gazebo-11/plugins
```
```bash
cd lightsfm
make
sudo make install
```

### Build
```bash
# The walking pedestrian plugin for Gazebo
colcon build --packages-select gazebo_sfm_plugin

# To train reinforcement learning agents for a path planning problem
colcon build --packages-select hospital_robot_spawner
```

### Run
```bash
ros2 launch hospital_robot_spawner gazebo_world.launch.py
ros2 launch hospital_robot_spawner start_training.launch.py
```
```bash
ros2 launch hospital_robot_spawner gazebo_world.launch.py
ros2 launch hospital_robot_spawner trained_agent.launch.py
```
