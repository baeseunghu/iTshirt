import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns

# 임의의 데이터 생성
np.random.seed(0)
x = np.random.randn(100)
y = 2 * x + np.random.randn(100)

# 데이터를 데이터프레임으로 변환
data = pd.DataFrame({'X': x, 'Y': y})

# 산점도 그리기
plt.figure(figsize=(8, 6))
sns.scatterplot(x='X', y='Y', data=data)
plt.title('Scatter Plot of X and Y')
plt.xlabel('X')
plt.ylabel('Y')
plt.grid(True)
plt.show()
