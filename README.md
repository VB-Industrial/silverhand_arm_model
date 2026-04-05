# silverhand_arm_model

Pure Silverhand arm model package for RViz visualization.

## What Is Inside

- `urdf/silverhand_arm.urdf.xacro` - top-level arm xacro
- `urdf/silverhand_macro.urdf.xacro` - reusable arm macro
- `meshes/` - STL meshes
- `launch/display.launch.py` - RViz and state publisher launch
- `rviz/silverhand_arm.rviz` - default RViz configuration

The package installs only xacro sources; generated `*.urdf` files are not tracked or installed.

Run the standalone arm view with:

```bash
ros2 launch silverhand_arm_model display.launch.py use_joint_state_gui:=true
```
