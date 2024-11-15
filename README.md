# MicroROS以太网传输数据

一共有三个需要注意的地方：

- 确保网卡驱动正确
- 确保STM32以太网正常驱动
- 确保传输层选用transport_udp.c文件
- 确保IP地址正确

调用命令：

```bash
ros2 run micro_ros_agent micro_ros_agent udp4 --port 8888 -v6
```

`CMakeLists.txt`文件中的 `YOUR_MICROROS_API_PATH` 路径需要根据你的MicroROS位置放置。
