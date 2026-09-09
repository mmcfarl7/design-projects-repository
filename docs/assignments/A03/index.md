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

Here is when I applied the simulation and thus resulted in the forces you can observe in the images and video below. Look at the legend to further understand what is occurring to the beam. Thankfully Creo also allows for Simulation Reports, which I've added below for your observatoni.

<img width="430" height="570" alt="IMG_2393" src="https://github.com/user-attachments/assets/34e472f7-0ae9-49d9-aded-bfee48df4e42" />

<img width="430" height="570" alt="IMG_2394 (1)" src="https://github.com/user-attachments/assets/a8968797-4684-4a9e-9f92-b149eb405027" />

<img width="430" height="570" alt="IMG_2395" src="https://github.com/user-attachments/assets/1ca91afa-f3ef-4a32-9360-3aee45bd3351" />

<img width="430" height="570" alt="IMG_2396" src="https://github.com/user-attachments/assets/cf6b04e6-b66c-4f54-ae2b-36b6c8e03b7a" />

Here's a video of me applying the simulation. As you can see most of the beam is under high strain while the fixed point has the most color distribution.

https://github.com/user-attachments/assets/5f43ad8a-b054-4740-8a6d-69a727f951aa

## Communicate

Fortunately, this beam design DOES satisfy the aluminum Max Stress test of 40 ksi. The safety factor calculated is shows as 40 ksi divided by the max FEA stress of 1.71075 ksi which gives a safety factor of 23.4, which is incredibly large. Calculating the percent difference based off of the deflection in the FEA analysis was 2.20235 times 10 to the -5th power subtracted from the allowed deflection of 0.009 inches divided by the allowed deflection, then finally multiplied by 100 to equal 99.735% difference.

<img width="300" height="70" alt="image" src="https://github.com/user-attachments/assets/16b297c9-a185-41ee-81c3-83c0123bf0c1" />

<img width="490" height="570" alt="IMG_2410" src="https://github.com/user-attachments/assets/f99e1c42-9798-41dc-8145-511cbdd0d5a1" />

<img width="430" height="570" alt="IMG_2411" src="https://github.com/user-attachments/assets/73701d59-38b7-4a5e-9568-cb6d7d0aa000" />

<img width="570" height="430" alt="IMG_2412" src="https://github.com/user-attachments/assets/c5d44fa1-9796-4150-8d96-15ef0704283b" />

<img width="570" height="430" alt="IMG_2413" src="https://github.com/user-attachments/assets/b18614b5-5b8a-441f-a9de-d74f6fe18e50" />

<img width="430" height="570" alt="IMG_2414" src="https://github.com/user-attachments/assets/9cf88788-7461-4cc4-9ece-dbc8de73abd1" />

I was asked near the end of this assignment to imagine if I had a circular hole in a flat bar subjected to tension with a stress concentration factor of K=3. Using the FEA nominal stress of 1.71075 ksi, the estimated peek stress of the hole as per the Machine Handbook would be PEAK=K multiplied by Nominal Stress which would be 3 times 1.71075, which equals 5.13 ksi.

The allowable stress is 40 ksi, so n=40/5.13 which gives us 7.79. Therefor the beam would still pass the stress requirement even with the pin-hole concentration.

### Lessons Learned

I've learned much. Firstly, I've learned how to do simulations in Creo, which was a pain to do on the factor that my current setup as per the time of making this report was not powerful enough to run Creo Simulations. Therefore, most of the work you've seen here is done on more powerful computer monitors in the classroom, even outside class hours. Along with that, as of the time I was working midway on this assignment around the 3rd hour mark when my Creo license expired so I had to redownload the latest Creo software with my student account to continue using Creo modeling software for free, else I'd have to pay thousands of dollars a year to do my work at home instead of in the classroom. Thankfully, with all those issues averted and out of the way, I was able to get all the work done, learned how to do simulations, and I even was able to see in depth how forces and deformations can be shown in model projections instead of in real time, which really shows how far some technology has come.
Total time to complete: 6 hours over the course of multiple days.
