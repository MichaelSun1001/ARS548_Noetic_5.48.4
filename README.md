# **单个侧视角雷达**

1、自己电脑的IP要配置为10.13.1.166，默认网关10.13.1.1，子网掩码255.255.255.0。
2、软件使用时，要关掉防火墙。
3、雷达IP：10.13.1.113

# **编译**

rm build/ devel/ -fr
catkin_make --pkg ars548_msg
catkin_make -j20

# **运行**

source devel/setup.bash
roslaunch ars548_process ars548_process_side.launch
