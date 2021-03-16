```python
import numpy as np
```



# 保存.npy文件
```python
arr = np.array([[1, 2], [3, 4]])
np.save("../data/arr.npy", arr)
print("save .npy done")
```



# 读取.npy文件

```python
arr = np.array([[1, 2], [3, 4]])
np.load("../data/arr.npy")
print(arr)
print("load .npy done")
```

