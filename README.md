# Analytical-Dynamics-Project-2
This project will
## Solving for M(q)
First the center of mass is needed and is taken from the position vector. The following equations are taken from the diagram.

  ![image](https://github.com/user-attachments/assets/8c977780-3259-4900-91ea-cbae055dbe4b)
After having the equations for each component each componets derivatives can be taken.
  ![image](https://github.com/user-attachments/assets/4dbdd5b8-2062-42ea-a882-77e9524bb366)
  ![image](https://github.com/user-attachments/assets/c469c53a-7b6c-42d0-8a28-5c6a94c908fe)

Now subsituiting the equstions into the equation below allows for the derivation of M
  ![image](https://github.com/user-attachments/assets/3fe89aff-0a40-4825-9966-e3e170a8bccb)
After using the equation above the subsition looks like the expressions below:
  ![image](https://github.com/user-attachments/assets/f0d43415-6604-4ad6-9563-4aaa9ef7ae49)
  ![image](https://github.com/user-attachments/assets/89af6bbe-c5ea-4a55-bc9c-0db2e72e1cee)

Then putting the equations in matrix form the M matrix can be derived below if terms are combined and put into a matrix.

  ![image](https://github.com/user-attachments/assets/02ef2f9e-869f-4046-af35-e5dc76d3e6e3)

## Verify equations of motion
Given:
![image](https://github.com/user-attachments/assets/774d7171-5116-4da5-bcb7-df8a55f2d9b6)
![image](https://github.com/user-attachments/assets/6bf5b842-98bc-480b-89ab-a52b46459bff)
![image](https://github.com/user-attachments/assets/f761cb58-9e5d-41de-bfb0-3445abf59de6)
![image](https://github.com/user-attachments/assets/d2e088ec-b504-4b8b-8d7d-47fcd6af9efd)




The lyapunov function is also given in 8.9 example:

In order to verify the equations of motion the equations need to match the given expression below:

Due to the problem not stating anything dealing with potential energy the lagrange equation is equal to kinetic energy. Using the kineitc energy and lagrange equationa and equaling it to Q will allow for the equations of motion to be derived below. 



Solving the partials will allow for the equation to match the expression that was given above. The code shows this with the matrix as it is given instead of just an M variable as done before. So the equation of motions that were derived matches the given expression for the problem and it is verfied in the code.  

## Program and carry out numerical simulations using control laws
Intial conditions



### Part 1: Running at least 100 Monte-Carlo simulations
In the code the simulation was ran 100 times and then the success rate was given to test the global stability of control of the system. After running the code using the control law equations the success rate was 100%. This meant that the system goes back down to it's equilbrium point. However, this can be considered strange to have each trial to be 100% successful. So the code could be incorrect or the inital conditions are to small and there's not enough trials. The graph below shows the frequency and the sucess rate for each trial. 



### Part 2: Use a Fixed set of initial condition, compare the performance of the two control laws by showing the curves of  ̇q and the corresponding controls Q1 and Q2.
Using the inital conditions already in the code. The plots for needed for this section can be determined. The goal of this was to understand how the inital conditons influence Q1 and Q2. For the velocity the velocity decrease indicates that how quickly the system slows down. Then the control plot demostrates how the hard the system has to work or how much effort the system has to do. In the code the plots were able to be plotted and compared with example 8.9. The plot below shows Q1 and Q2 and there differences in more depth by using different colors. 


### Part 3: Introducing an Inertia Matrix Error For Q2




