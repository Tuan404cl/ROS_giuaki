# ROS_giuaki
Kiểm tra giữa kì môn lập trình ROS
Chay file lauch
    colcon build --packages-select tank
    source install/setup.bash
    export GAZEBO_MODEL_PATH=$GAZEBO_MODEL_PATH:~/tank_ws/install/tank/share
    ros2 launch tank gazebo.launch.py

Dieu khien dong co robot
    ros2 run teleop_twist_keyboard teleop_twist_keyboard

Dieu khien tay may gan tren robot
    python3 src/tank/scripts/keyboard_control.py

Khoi dong camera
    ros2 run rqt_image_view rqt_image_view
