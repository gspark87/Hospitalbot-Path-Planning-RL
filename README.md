# Hospitalbot-Path-Planning-RL

```bash
colcon build --packages-select gazebo_sfm_plugin

colcon build --packages-select hospital_robot_spawner


### Run

```bash
ros2 launch hospital_robot_spawner gazebo_world.launch.py
ros2 launch hospital_robot_spawner start_training.launch.py

```bash
ros2 launch hospital_robot_spawner gazebo_world.launch.py
ros2 launch hospital_robot_spawner trained_agent.launch.py
