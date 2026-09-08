# A3 – Parametric and FEA

## Objective
Objectives:

-Use axial deflection modeling to design its dimensions

-Use parametric design to determine a bars length

-Introduce you to FEA (Finite Element Analysis)

-Introduce you to linking dimensions to appropriate parameters in CAD.

-Compare and contrast the different analysis

## Analyze
First thing we had to do was to create a cross-sectional area. For me, I chose to use a 1-inch height by 0.5-inch width. Using the equation for Hooke's Law from the Machinery's Handbook, I was able to determine the length by rearranging the equation 

(Max deformation) = (Force X Length)/(Cross Sectional Area X Young Modulus) 

into

(Length) = (Max Deformation X Cross Sectional Area X Young Modulus)/(Force)

So, to plug in the numbers, Max Deformation is the parameter 0.009 inches, Cross Sectional Area is 0.5 inches by 0.5 inch so the cross-sectional area is 0.250 inches squared. And lastly is Young Modulus and Force, which are 10 X 10^6 psi and 400 lbf respectively, chosen as the median of the largest and smallest ranges of young modulus and force.

Calculations would show that L = 56.25 inches here:

<img width="250" height="250" alt="image" src="https://github.com/user-attachments/assets/d12d7bf3-5e83-4245-9b56-b9993454c91e" />



## Decide
I created the beam as shown below with the parameters I explained above. I then initiated the change in materials from default on Creo to aluminum as per the guidelines, and thankfully Creo has an Aluminum material in their library, Aluminum 2014.mtl to be exact. The Poisson's ratio and density and even the Young Modulus were correct, so I used that for my beam. Now onto the forces...

<img width="1000" height="370" alt="image" src="https://github.com/user-attachments/assets/fef1de7b-10c9-44dc-a9da-098436183cc1" />

<img width="250" height="250" alt="image" src="https://github.com/user-attachments/assets/27c8ce61-02c9-4252-8415-e5dc4f99f1b9" />

<img width="1000" height="850" alt="image" src="https://github.com/user-attachments/assets/e666c2c9-3579-4fe5-9795-e5b21b327361" />

Here you can see I applied a fixed position to the left side of the beam and a 400 lbf tensile force to the right side of the beam.

<img width="1200" height="250" alt="image" src="https://github.com/user-attachments/assets/c2c649ca-924f-4657-9218-64d66a605647" />



## Communicate

