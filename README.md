# Stabilizing the Pendulum

## 轻微扰动稳定问题

### 问题描述
- **初始状态**：摆从一个轻微倾斜的位置开始。
- **目标**：通过控制小车的运动使摆稳定在竖直向上位置。

### 文件夹内容
- 代码
- 视频
- 训练好的模型

## 起摆稳定问题

### 问题描述
- **初始状态**：摆从竖直向下的位置开始。
- **目标**：通过控制小车的运动将摆摆动到竖直向上位置并稳定。

### 注意事项
运行此代码时，需要在`inverted_pendulum_v4.py`的原始文件中的`reset_model`方法中的`self.set_state(qpos, qvel)`上面加上一行代码：

```python
qpos[1] = np.pi
```

目的是在初始时使倒立摆竖直向下。