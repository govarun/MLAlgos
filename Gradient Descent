import numpy as np
import matplotlib.pyplot as plt
x = np.array([1, 2, 3, 4, 5, 6, 7, 8, 9, 10])
y = np.array([0, 1, 5, 6, 10, 9, 13, 16, 5, 18])
plt.scatter(x, y)
plt.show()
w = np.random.rand(2, 1)
print(x)
y_pred = w[0]*x + w[1]
plt.plot(x, y_pred)
for j in range(1000):

    derivm = -2 * (((y - y_pred) * x).sum())
    derivc = -2 * ((y - y_pred).sum())
#     print(">", end = " ") 
#     print(derivm)
#     print(">", end = " ")
#     print(derivc)
    alpha = 0.0001
    w[0] = w[0] - alpha * (derivm)
    w[1] = w[1] - alpha * (derivc)
    y_pred = w[0]*x + w[1]
    loss = ((y - y_pred) * (y - y_pred)).sum()
    print(loss)
    plt.plot(x, y_pred)

plt.scatter(x, y)
plt.show()
