Biazon, Gian Alfred V. Programming-Assignment-2

This repository contains solutions to identify the codes and functions incorporated in the Numpy Library and to be able to apply and use the different codes and functions in creating a Python program using the Numpy Library.

Problem #1 - NORMALIZATION PROBLEM - Subtracting the data from the mean and scaling means dividing with its standard deviation. Mathematically, normalization can be expressed as Z = Z = (x - mean) / standard deviation

Code:

      import numpy as np
      RANDOM = np.random.random((5,5))
      print("Random array: ")
      print(RANDOM)
      print()

      mean_RANDOM = RANDOM.mean()
      std_RANDOM = RANDOM.std()
      RANDOM_normalized = (RANDOM - mean_RANDOM) / std_RANDOM 

      print("Normalized array: ")
      print(RANDOM_normalized)

  Output:
      <img width="588" height="287" alt="image" src="https://github.com/user-attachments/assets/6a9f3eac-14e1-4f70-a0c2-3d049dcc2448" />

  Analysis:
          The most important part of this problem is the mathematical formula, which subtracts the data and the mean to move the distribution around zero, and normalizes the data by dividing by the standard                 deviation to produce a uniform spread. This conversion takes the original array and converts it into a standard normal distribution with a mean value of 0 and standard deviation of 1, which is the 
          critical output demanded by the problem.


Problem #2 - DIVISIBLE BY 3 PROBLEM - Create a 10x10 ndarray made up of squares of the first 100 positive integers, then take the elements divisible by 3.

Code:

      square = Positive100 ** 2 
      Ten_by_Ten = square.reshape(10,10) 
      print("A= ")
      print(Ten_by_Ten)
      print()

      divisible = Ten_by_Ten % 3 == 0 
      Three = Ten_by_Ten[divisible] 
      print("Elements divisible by 3: ")
      print(Three)
      print()

      np.save('Three.npy',Three)

Output:
      <img width="649" height="350" alt="image" src="https://github.com/user-attachments/assets/582e3bcb-d24b-43d9-9b5e-13c22bb9ed0a" />

Analysis:
        The most important part of this problem is boolean indexing with the expression "Ten_by_Ten % 3 == 0", which forms a variable that selects all the elements in the 10×10 array whose remainder when divided          by 3 is zero. This method filters and picks only those elements that satisfy the divisibility condition efficiently without any need for explicit loops, taking advantage of NumPy's vectorized operations           for best performance. The array produced has exactly the squares of integers that are multiples of 3, which is the core output needed by the problem.

