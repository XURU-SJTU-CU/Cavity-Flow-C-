# Cavity-Flow-C++
2D Cavity flow - Finite-Volume-Method, SIMPLE algorithm, collocated grid, Re = 100, 400, 1000, 10000

# Governing Equations

Momentum equation:

![image](https://user-images.githubusercontent.com/33889393/152107755-4f2b93e6-d77a-41f9-aa04-57864d0da759.png)

Continuty equation:
![image](https://user-images.githubusercontent.com/33889393/152107919-4d321ba7-c817-4139-aeca-a34a8ad78b6f.png)

The expanded form in 2D can be written as following
![image](https://user-images.githubusercontent.com/33889393/152108005-ec520141-5dee-4737-aa2a-b6f700d74b93.png)

Since we use finite volume method, a control volume is specified as the following picture
![image](https://user-images.githubusercontent.com/33889393/152108417-40802a36-18c7-4032-afc6-ac16b063fd2b.png)






Note: 
1. the coefficient for velocity matrix denoted by 
C_P_coeff[i][j], C_E_coeff[i][j], C_W_coeff[i][j], C_N_coeff[i][j], C_S_coeff[i][j]

2. the coefficients for pressure matrix denoted by
K_P_coeff[i][j], K_E_coeff[i][j], K_W_coeff[i][j], K_N_coeff[i][j], K_S_coeff[i][j]

