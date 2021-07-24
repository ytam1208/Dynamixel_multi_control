# Dynamixel_multi_control

---

## Branch 
- master(default)
- Melodic.ver(Ubuntu 18.04 LTS)
- Kinetic.ver(Ubuntu 16.04 LTS)

---

|Series|version|Use|
|------|------------------------------------------------------------------------------------------------------------|---|
|AX|AX-12W, AX-12/12+/12A, AX-18F/18A|O|
|RX|RX-10, RX-24F, RX-28, RX-64|O|
|EX|EX-106+|O|
|MX|MX-12W, MX-28, MX-28(2.0), MX-64, MX-64(2.0), MX-106, MX-106(2.0)|O|
|XL|XL320, XL330-M077, XL330-M288, XL430-W250|O|
|XC|XC430-W150, XC430-W240|O|
|XM|XM430-W210, XM430-W350, XM540-W210, XM540-W270|O|
|XH|XH430-W210, XH430-W350, XH430-V210, XH430-V350|O|
|XW|XW540-T140-R, XW540-T260-R|O|
|PRO-L|L42-10-S300-R, L54-30-S500-R, L54-30-S400-R, L54-50-S500-R, L54-50-S290-R|O|
|PRO-M|M42-10-S260-R, M54-40-S250-R, M54-60-S250-R|O|
|PRO-H|H42-20-S300-R, H54-100-S500-R, H54-200-S500-R|O|
|P-Series|PH54-200-S500-R, PH54-100-S500-R, PH42-020-S300-R, PM54-060-S250-R, PM54-040-S250-R, PM42-010-S260-R|O|
|Dual axle DYNAMIXEL products|2XL430-W250-T or 2XC430-W250-T|O|


reference: http://wiki.ros.org/dynamixel_workbench

---

## Setting
- Multi Id array = {ID 1....ID n}
- Sync multi control dynamixel


---

## Operate command

```
roslaunch dynamixel_workbench_ros_control example.launch
```

---

## ROS service example 

```
rosservice call /dynamixel_workbench/dynamixel_command "command: ''
id: 1
addr_name: 'Goal_Position'
value: 2048"
```
reference: https://emanual.robotis.com/docs/en/software/dynamixel/dynamixel_workbench/#position-controller
