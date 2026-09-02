# A02 - Truss Stress Analysis

## Objective

The objective of this project was to design and analyze a simple truss structure capable of supporting the applied loads shown in Figure 1. The truss was designed using the given geometric constraints and loading conditions, while keeping the cross-sectional area of every member identical. The final design was then modeled in  a CAD program (I used Creo) to verify that the selected geometry and member size could satisfy the required strength and safety factor.

There was also a bulleted list of objectives, which I will include here:

<img width="1170" height="648" alt="image" src="https://github.com/user-attachments/assets/4a6be2e5-6605-4c13-a584-b3bdeada3b9f" />


### Original Design Constraints:

<img width="1442" height="1028" alt="image" src="https://github.com/user-attachments/assets/93b1a6a1-e429-414d-a7ce-abe74403ddb9" />


---

## Analyze

The truss geometry was selected based on the dimensions given in Figure 1, including the required spacing between the supports and the applied loads at points C and D. I analyzed the truss by determining the support reactions and internal forces in each member so that the most heavily loaded member could be identified, which turned out to be the inner diagonal supports. Then the largest internal force calculated was then used to determine the minimum required cross-sectional area using the yield strength of the selected A500 structural steel and the required safety factor.

### Work and Calculations
<img width="536" height="714" alt="IMG_2318" src="https://github.com/user-attachments/assets/115debef-2b1b-46ca-9658-566a1aead440" />
<img width="536" height="714" alt="IMG_2319" src="https://github.com/user-attachments/assets/18e3574b-a874-4c03-926c-1eb0e02ee732" />
<img width="536" height="714" alt="IMG_2320" src="https://github.com/user-attachments/assets/9227c37b-e5a2-4d1b-85d0-d20fdf5d7e4c" />


The analysis showed that the largest internal member force occurred in the inner diagonal members ED and EA. This force was used as the controlling load for selecting the cross-sectional area of the truss members.

After doing all the calculations later in the day, I felt really tired, so I felt that one thing I definetly could've improved on is taking my time with projects like these to prevent burnout and excessive frustrating emotions during the time of these calculations. These calculations weren't exactly difficult, they were simply very time consuming, and I had other things I wanted/had to do, so doing everything all at once, even when it was planned out, became somewhat difficult to manage.

---

## Decide

I selected the final truss geometry because it is simple, symmetric, and provides a stable load path between the supports and the applied loads (also it was kinda fairly obvious what the design was supposed to be). All truss members were designed with the same cross-sectional geometry, as required by the assignments parameters. Based on the calculated minimum area, I selected a 0.55 in × 0.55 in cross section for each member, providing a cross-sectional area of 0.3025 in² and satisfying the required safety factor.

### Final Model and Model Process:

<img width="1216" height="872" alt="image" src="https://github.com/user-attachments/assets/37606350-320b-4153-bbb9-12f73e29e753" />

<img width="2026" height="872" alt="image" src="https://github.com/user-attachments/assets/c2e17274-3c43-4454-9bd6-299457a16636" />

<img width="450" height="408" alt="image" src="https://github.com/user-attachments/assets/f476e936-7c65-44a2-b9f1-190c51e8d9d9" />

### KEYNOTE: The measurements seen above are in inches, converted from meters from my calculations seen in the previous header, since Creo's default was inches and I chose instead of converting to mm I would just convert my paper measurements to inches for Creo's ease of use by default settings.

The selected member area is greater than the calculated minimum required area, providing additional margin while keeping the design simple to manufacture and model.
I had also calculated that the total weight of the truss system, when the properties of A500 steel was applied, was roughtly 10% higher than my estimated calculations as show above on page 3. 

---

## Communicate

The final truss was created as a 3D CAD model using the geometry and member dimensions determined during the analysis. A500 structural steel was assigned as the material, and the same 0.55 in × 0.55 in cross section was used for each truss member. The CAD model provides a visual representation of the final design and allows the mass properties and predicted weight of the truss to be evaluated.

### Engineering lesson: I learned how to design a simple truss system, to calculate different aspects of said truss system including all the forces in and around it and the stress/strain via the yield strength of the material involved. I also learned digital modeling of said truss system and the frustrations that digital software come with based on how they can turn simple items such as this truss system into something far too complex to model.

The CAD model was created without the connecting pins because the pins were analyzed separately. The completed model demonstrates how the analytical calculations were translated into a physical three-dimensional design. 

To compare the model from my calculations, I have learned that my model would do well considering the cross-sectional area is slightly bigger at 0.3025 in² rather than my calculated 0.274 in². It also proved to weight just about as much as my calculations. While not shown on paper since the calculations were done digitally in a computer language that is frustrating to display on Github, I have included a small screenshot where you can see the label "Mass" which is roughly 11 pounds, which is close to my calculated formula of approximately 10 pounds.

<img width="504" height="142" alt="image" src="https://github.com/user-attachments/assets/659b5d06-b88a-43c5-8041-b09658097761" />

I would also like to mention that there was no A500 steel on Creo, at least none that obviously made itself known, so I had to improvise and use the average statistics of A500 steel to customize the material stats of the model.

# Resources:

Google.com

https://www.beamdimensions.com/materials/Steel/ASTM/ASTM_A500/   (Had to watch an ad for this one)

Class notes

https://www.desmos.com/calculator   (Calculator I used to keep track of all the variables)

Page 147 of the Machinery's Handbook Guide, 32nd edition (I had the wrong textbook at the time but it had some vaulable data surrounding pin shear stress)
