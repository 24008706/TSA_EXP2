# Ex.No: 02 LINEAR AND POLYNOMIAL TREND ESTIMATION
Date:
### AIM:
To Implement Linear and Polynomial Trend Estiamtion Using Python.

### ALGORITHM:
Import necessary libraries (NumPy, Matplotlib)

Load the dataset

Calculate the linear trend values using least square method

Calculate the polynomial trend values using least square method

End the program
### PROGRAM:
A - LINEAR TREND ESTIMATION
```
import numpy as np
import matplotlib.pyplot as plt

x = np.array([1, 2, 3, 4, 5, 6])
y = np.array([10, 20, 25, 30, 40, 50])

m, c = np.polyfit(x, y, 1)
trend = m*x + c

plt.plot(x, y, 'o', label='Original Data')
plt.plot(x, trend, label='Linear Trend')
plt.title('Linear Trend Estimation')
plt.xlabel('X')
plt.ylabel('Y')
plt.legend()
plt.show()

print("Linear Trend Values:", trend)
```
B- POLYNOMIAL TREND ESTIMATION
```
import numpy as np
import matplotlib.pyplot as plt

x = np.array([1, 2, 3, 4, 5, 6])
y = np.array([10, 20, 25, 30, 40, 50])

coeff = np.polyfit(x, y, 2)
trend = np.polyval(coeff, x)

plt.plot(x, y, 'o', label='Original Data')
plt.plot(x, trend, label='Polynomial Trend')
plt.title('Polynomial Trend Estimation')
plt.xlabel('X')
plt.ylabel('Y')
plt.legend()
plt.show()

print("Polynomial Trend Values:", trend)
```
### OUTPUT
A - LINEAR TREND ESTIMATION

<img width="892" height="595" alt="image" src="https://github.com/user-attachments/assets/4202fdd6-d916-4093-bb10-68c4f6ce41f0" />

B- POLYNOMIAL TREND ESTIMATION

<img width="997" height="606" alt="image" src="https://github.com/user-attachments/assets/0d03027f-dafe-4d15-918c-28a712e14675" />

### RESULT:
Thus the python program for linear and Polynomial Trend Estiamtion has been executed successfully.
