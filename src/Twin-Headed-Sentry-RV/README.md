# Double-headed-Sentinel
该双头哨兵视觉代码修改自陈君的RM_VISION代码，在此十分感谢陈君的开源代码</br>
本项目的基本思路为通过发布两个detector节点，对装甲板进行识别后进行发送装甲板信息，中间会经过choose节点的选择转发到tracker，最后tracker再对装甲板信息进一步处理并向下发送到电控端</br>
</br>

相机标定信息应当存放在 hik_camera/config/camera_info.yaml 及 hik_camera_second/config/camera_info.yaml

相机曝光时间修改位于/rm_vision/rm_vision_bringup/config/node_params.yaml

坐标信息修改位于 /rm_gimbal_description/urdf/rm_gimbal.urdf.xacro