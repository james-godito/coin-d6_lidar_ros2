sudo cp sc_mini.rules /etc/udev/rules.d
sudo udevadm control --reload-rules
sudo udevadm trigger
ls -l /dev/sc_mini
% Should show: lrwxrwxrwx 1 root root 7 Oct 29 11:43 /dev/sc_mini -> ttyUSB0
ros2 run m1ct_d2 m1ct_d2
% Then open Rviz2 and change laserscan source
