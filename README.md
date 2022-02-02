# Cavity-Flow-C++
2D Cavity flow - Finite-Volume-Method, SIMPLE algorithm, collocated grid, Re = 100, 400, 1000, 10000

# Governing Equations

Momentum equation:

![image](https://user-images.githubusercontent.com/33889393/152107755-4f2b93e6-d77a-41f9-aa04-57864d0da759.png)

Continuty equation:
![image](https://user-images.githubusercontent.com/33889393/152108712-1814b1c6-2bf4-4600-b207-06c6392b5fb4.png)


The expanded form in 2D can be written as following

![image](https://user-images.githubusercontent.com/33889393/152108672-08dd86db-42f0-490f-a591-c0f748ccd986.png)


Since we use finite volume method, a control volume is specified as the following picture
![image](https://user-images.githubusercontent.com/33889393/152108760-e4c5567a-41bd-47f4-a2a0-9ada7b89ced9.png)

The discretized equation can be expressed as following using upwind-scheme

![image](https://user-images.githubusercontent.com/33889393/152108988-7ed45f7f-a742-4105-b04f-b9d448a75c79.png)
where the coefficients are expressed as:
![image](https://user-images.githubusercontent.com/33889393/152109076-00f148d3-6f48-4a11-ba22-df37ab63512e.png)

For the pressure equation:
![image](https://user-images.githubusercontent.com/33889393/152109205-19288fe4-9ea1-4347-adf1-29d48ab89809.png)






Note: 
1. the coefficient for velocity matrix denoted by 
C_P_coeff[i][j], C_E_coeff[i][j], C_W_coeff[i][j], C_N_coeff[i][j], C_S_coeff[i][j]

2. the coefficients for pressure matrix denoted by
K_P_coeff[i][j], K_E_coeff[i][j], K_W_coeff[i][j], K_N_coeff[i][j], K_S_coeff[i][j]

