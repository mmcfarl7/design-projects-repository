# A4 – Motor Mount

## Objective
The objective of this project was to design and develop a 3D-printable motor mount capable of supporting the specified DC gear motor while remaining within the required strength and deflection limits. The motor mount was designed to attach to a rigid wall and was divided into two primary structural features.

The first feature supports the motor and transfers the applied shaft load into the remainder of the mount. The second feature connects the motor-supporting section to the rigid wall. Both features were initially modeled as cantilever beams so that beam-bending equations could be used to determine the required cross-sectional geometry.

<img width="300" height="150" alt="image" src="https://github.com/user-attachments/assets/a9df731b-f487-412a-93e5-0be8c4d2d6c7" />

The PETG material properties used for the preliminary calculations were obtained from the provided material-property spreadsheet. The average tensile yield strength was taken as 44.8 MPa, while the average Young's modulus was taken as 3.03 GPa, or 3030 MPa.

## Analyze
# Feature 1 & 2
The motor mount was separated into Feature 1 and Feature 2 to simplify the structural analysis.

Feature 1 was treated as a horizontal cantilever supporting the applied motor load. According to the provided figure, the 300 N load acts along the positive x-axis at the free end of the feature.

Feature 2 was treated as a second cantilever that transfers the loading from Feature 1 into the rigid wall.

This simplified approach allows the bending stress and deflection of each feature to be calculated using standard beam-bending equations.

Utilizing Stress and Deflection equations as shown below, I created a basic sketch of my original approximated/estimated measurements. Since I was utilizing similar equations between these features for the same purposes, I reused the deflection and yield-strength equations between the two features.

During the mathematical process I observed it wasn't the yield strength of the material that was governing the thickness, it was the deflection parameters. Along with the equations is everything else needed to solve the problems from FBD's to legends of Known's and Uknown's to symbolically solving for the parameters and finally solving for the numerical solutions.

<img width="400" height="500" alt="IMG_2490" src="https://github.com/user-attachments/assets/51bdfabf-9da9-4220-926e-24211f1bd6b7" />

<img width="400" height="500" alt="IMG_2491" src="https://github.com/user-attachments/assets/521bce39-56f7-41db-919c-30f54586b20e" />

I didn't realize this far into the process that my measurements were skewed towards a rather impractical looking Motor Mount, but I persevered and continued using these original dimensions.

It wasn't until I reached the next segment that I suddenly questioned what the final appearance would look like.
# SKETCH

<img width="400" height="350" alt="IMG_2492" src="https://github.com/user-attachments/assets/2abdc12d-121d-400d-a76a-0787ffaeefe2" />

Looking at my dimensions, this was the part I questioned the appearance and practicality of my design, but I was already in the deep end, so I figured I'd model it and see how it looks outside the pencil sketch. I asked myself "What could possibly go wrong?"
## Decide
# CAD MODEL
The next day, after modeling, I realized things were VERY WRONG.

<img width="570" height="430" alt="IMG_2487" src="https://github.com/user-attachments/assets/031c521f-8574-4869-990c-aa75c9c13b3a" />

<img width="430" height="570" alt="IMG_2486" src="https://github.com/user-attachments/assets/5ec4ae21-af52-46f1-bdac-0d4718d533b2" />

<img width="430" height="570" alt="IMG_2485" src="https://github.com/user-attachments/assets/70252ad5-fd61-4436-9733-6d718e66f86d" />

If it wasn't plainly obvious, my model was rather... FAT. I questioned how I could've gotten to such an unusual shape. I double checked my math; it was accurate in my head. I started playing around with new dimensions and tried doubling my original dimensions of 50 mm to 100 mm and tested to see how the thickness would appear then. After a bit of troublesome math, I discovered that the thickness would be roughly 25 mm, which is 1/4th the length and width of the model, which was more appealing, but then it made the hole for the motor mount appear small.

Circling back, I wondered if it was because of the Safety Factor being so large that the appearance was skewed to be fatter. Just by looking at the model I questioned if you could bend the cantilever without it snapping due to its sheer mass. Alas, this was not graded on appearances, it's graded on logic, math, and hypothetical/theoretical performance. An initial brainstorm doesn't make this model a failure. It will pass, if it was printed out, it would just be incredibly inefficient. 

## Communicate

# Lessons Learned

Ultimately, the mistake I made was the initial measurements and my stubbornness to not change the parameters later in development when I was drawing the isometric sketch. If I had gone back and tried new lengths, it wouldn't have required too much re-calculating, and maybe then the model would look more appealing. I do wonder if there was perhaps a better method to achieve the end goal, like by adding thin triangular supports in the corners between the beams. Perhaps with the addition of support in the structure, the model would be more finished and appealing visually. Alas, I stuck it through. I hope that despite the visual disgust of this model I learn to redesign things to be not only functional, but more appealing to the eye.


# Resources + Part file

https://www.google.com/url?q=https://www.matweb.com/search/DataSheet.aspx?MatGUID%3D4de1c85bb946406a86c52b688e3810d0%26ckck%3D1&sa=D&source=editors&ust=1789571883369363&usg=AOvVaw30RjDYFs1H_JgwK_y-ha9M

-(PETG data in a spreadsheet)

https://www.google.com/url?q=https://www.omc-stepperonline.com/brushed-24v-dc-gear-motor-3-6kg-cm-46rpm-w-99-5-1-planetary-gearbox-pa28-28245800-g100&sa=D&source=editors&ust=1789571883368309&usg=AOvVaw2F7skO1DjTZwHhcHfMCaag

-(The Motor in question)

<img width="600" height="300" alt="image" src="https://github.com/user-attachments/assets/8edb833c-f3b5-4146-aacb-46adc639a63d" />

-(An appendix of the motor.)

[a4_motor_mount.prt.zip](https://github.com/user-attachments/files/32297308/a4_motor_mount.prt.zip)

-(The final part design)
