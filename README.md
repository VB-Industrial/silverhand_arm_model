# silverhand_arm_model

Чистый пакет модели руки SilverHand для визуализации в RViz.

## Что внутри

- `urdf/silverhand_arm.urdf.xacro` - верхнеуровневый xacro для руки
- `urdf/silverhand_macro.urdf.xacro` - переиспользуемый макрос руки
- `meshes/` - STL-меши
- `launch/display.launch.py` - запуск RViz и state publisher
- `rviz/silverhand_arm.rviz` - конфигурация RViz по умолчанию

Пакет устанавливает только xacro-исходники; сгенерированные `*.urdf` файлы не отслеживаются и не устанавливаются.

Запустить отдельный просмотр руки можно так:

```bash
ros2 launch silverhand_arm_model display.launch.py use_joint_state_gui:=true
```
