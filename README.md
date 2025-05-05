# astr400b-homework-4-solved
**TO GET THIS SOLUTION VISIT:** [ASTR400B Homework 4 Solved](https://www.ankitcodinghub.com/product/astr400b-homework-4-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;102233&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;0&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;0&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;0\/5 - (0 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;ASTR400B Homework 4 Solved&quot;,&quot;width&quot;:&quot;0&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 0px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            <span class="kksr-muted">Rate this product</span>
    </div>
    </div>
<div class="page" title="Page 1">
<div class="layoutArea">
<div class="column">
We want to explore how each galaxy in the Local Group moves owing to the gravita- tional forces they each exert on each other. To do this, we need to compute the center of mass (COM) position and velocity vectors of each galaxy at any given point in time in the simulation.

The simulation is in Cartesian coordinates at all snapshots. At SnapNumber 0 (present day), the MW is located at the origin of this coordinate system x,y,z = (0,0,0). At later snapshots, the MW will move so it is no longer at the origin. Therefore, we need to track the COM motion of the MW, M31 and M33 to find their locations at future snapshots.

1 Beginning the Program: Defining the Class

You will be using a class structure for this solution set.

</div>
</div>
<div class="layoutArea">
<div class="column">
2

</div>
</div>
<div class="layoutArea">
<div class="column">
•

• •

• •

</div>
<div class="column">
Git pull on the course’s master repository to see an example script that you can use and modify for this assignment. CenterofMass Ex.py and centerofmass ex.ipynb contain the same information to guide you through this assignment.

Rename this script to CenterOfMass and save.

Functions in this program will call the Read function, so ReadFile is imported. Be sure

this file exists in the same directory.

You will once again need the files: MW 000.txt, M31 000.txt, M33 000.txt. In this program a CLASS called CenterOfMass has been defined.

class CenterOfMass:

A tutorial for classes in python can be found here: https://docs.python.org/3/tutorial/classes.html

Initialize the Class

</div>
</div>
<div class="layoutArea">
<div class="column">
Initialize your class so that each object will store data from the simulation file based on particle type.

</div>
</div>
<div class="layoutArea">
<div class="column">
1

</div>
</div>
</div>
<div class="page" title="Page 2">
<div class="layoutArea">
<div class="column">
def init (self, filename, ptype):

self.time, self.total, self.data = Read(filename)

self.index = np.where(self.data[’type’] == ptype)

self.m = self.data[’m’][self.index]

<ul>
<li>The index to help you store particle type has already been created for you. The particle masses have also been provided as an example.</li>
<li>Follow the same procedure as in ParticleProperties (Homework 2) to store the mass, position (x,y,z) of particles of a given type.</li>
<li>You must use “self” to refer to initialize values, eg. self.data[‘x’][self.index]. This stores the data for you when you create an object so that you do not have to read in the data each time you call a function.
The nomenclature “self” is used to refer to quantities that are common to the object. Each function you create must start with the word ”self” as an input. E.g.

def NewFunction(self, a):
</li>
</ul>
</div>
</div>
<div class="layoutArea">
<div class="column">
3

• •

• •

</div>
<div class="column">
Generic Definition of Center of Mass

Create a method called COMdefine that will generically return the 3D coordinates of the COM (position or velocity) of any given galaxy.

This method should take as input: the x,y,z coordinates of the particle position or velocity and the mass.

Remember that the first input for the function within a class is “self”

This function should return the x,y,z coordinates of the COM (position or velocity)

</div>
</div>
<div class="layoutArea">
<div class="column">
E.g. for each component of the position or velocity vector (like X) compute:

xCOM = Σximi (1)

Σmi

</div>
</div>
<div class="layoutArea">
<div class="column">
As shown in Fig. 1, this equation is generic: it would work if you input either the velocity or position vectors.

</div>
</div>
<div class="layoutArea">
<div class="column">
2

</div>
</div>
</div>
<div class="page" title="Page 3">
<div class="section">
<div class="section">
<div class="layoutArea">
<div class="column">
Example of the generic COM; XCOM = ximi mi

</div>
</div>
<table>
<tbody>
<tr>
<td></td>
<td></td>
<td></td>
<td></td>
<td colspan="2" rowspan="1">
<div class="layoutArea">
<div class="column">
Particles (mass=area) Center Of Mass

</div>
</div>
</td>
</tr>
<tr>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
</tbody>
</table>
<div class="layoutArea">
<div class="column">
4

2

0

2

4

</div>
</div>
<div class="layoutArea">
<div class="column">
42024 x-component of pos or vel [arbitrary units]

</div>
</div>
</div>
<div class="layoutArea">
<div class="column">
Figure 1: This picture presents an example of the generic definition of center of mass in a 2D plane. In each dimension of either the position or the velocity, the Eq. 1 is applied on the 25 particles (in blue) to determine their center of mass (in red). (Be careful that the data in your homework is three dimensional.)

</div>
</div>
<div class="layoutArea">
<div class="column">
3

</div>
</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
y-component of pos or vel [arbitrary units]

</div>
</div>
</div>
</div>
<div class="page" title="Page 4">
<div class="layoutArea">
<div class="column">
4 Refining the COM Position

Create a method called COM P that will call COMDefine to determine the center of mass (COM) position and velocity vectors of a given galaxy using particles of a given type.

<ul>
<li>The function should take as input: “self” and the tolerance (delta) that will decide whether the COM position has converged.</li>
<li>The function returns an array with the x, y, z coordinates of the COM position
While you have already created a generic function that returns the COM (COMdefine), you need to refine this COM position calculation iteratively (using successively smaller vol- umes) to make sure the position has converged. Do this by using the following steps.

Step 1: First Guess (see Fig. 2)
</li>
</ul>
<ul>
<li>Call COMdefine to compute a first estimate for the COM position vector (x COM, y COM, z COM) using all the particles of the desired type. Store the magnitude of that vector (r COM).</li>
<li>When referring to functions already definied in the Class you need to refer to “self” self.COMdefine.</li>
<li>Change the particle positions to the COM reference frame by subtracting the first guess COM position vector from the particle position vectors (self.x – x COM, etc).</li>
<li>Create an array that stores the magnitude of the new position vectors of all particles in the COM frame (r new).</li>
<li>Find the maximum 3D separation of the particles from the COM position in the COM frame and reduce it by half (r max). You will next refine the COM calculation using this smaller volume to make sure the COM position has converged.
Step 2: Refine the Guess (see Fig. 3)

Set up a while loop that continues while the difference between r COM and a new COM position (r COM2; computed using half the previous volume) is larger than some tolerance (delta), which you have set as an input value to this function.
</li>
</ul>
<ul>
<li>Pick an initial value for the change in COM position between the first guess (r COM) and the new one you will compute from half that volume (like 1000 kpc, so it will be larger than the input tolerance initially).</li>
<li>Set up a while loop, that continues while the change in r COM is larger than the tolerance (delta) that you want for convergence.</li>
<li>Store all particle positions and masses that have r new (3D separations in COM frame) less than half the maximum separation.</li>
</ul>
</div>
</div>
<div class="layoutArea">
<div class="column">
4

</div>
</div>
</div>
<div class="page" title="Page 5">
<div class="layoutArea">
<div class="column">
<ul>
<li>Compute the COM position using the particles in the refined volume and its magnitude (r COM2)</li>
<li>Compute the absolute magnitude of the difference in r COM2 to the older r COM.</li>
<li>Divide r max by half to refine the volume again and change all particle positions to the frame of reference of the new COM (x – x COM2, etc) and compute the magnitude of those vectors (reset r new).</li>
<li>Finally, reset the COM position vector (x COM, etc) to the newly computed COM2 vector and repeat the loop.
Step 3: Finally, return the converged COM Position Vector (x,y,z) as an array of astropy quantities in kpc, rounded to 2 decimal places.
</li>
</ul>
5 Computing the COM Velocity

Now that you know the COM position, you can compute the COM velocity by creating a method COM V.

</div>
</div>
<div class="layoutArea">
<div class="column">
•

• •

•

6

1.

2.

</div>
<div class="column">
Store the velocities of all particles that are within 15 kpc from the COM position. Note that you already initialized self.vx, self.vy, self.vz in the beginning of the class structure so you will only have to mask these based on the particles within 15 kpc.

Use COMdefine to compute and store the COM velocity.

Return the COM Velocity Vector (vx, vy, vz), as an array of astropy quantities in km/s

rounded to two decimal places.

The end of the provided example scripts show you how to create an object of the class and apply the methods of the class to that object (i.e. call COM P on the MW’s data file).

Testing Your Code

What is the COM position (in kpc) and velocity (in km/s) vector for the MW, M31 and M33 at Snapshot 0 using Disk Particles only (use 0.1 kpc as the tolerance so we can have the same answers to compare) ? In practice, disk particles work the best for the COM determination. Recall that the MW COM should be close to the origin of the coordinate system (0,0,0).

What is the magnitude of the current separation (in kpc) and velocity (in km/s) between the MW and M31? Round your answers to three decimal places. From class, you already know what the relative separation and velocity should roughly be (Lecture2 Handouts; Jan 16).

</div>
</div>
<div class="layoutArea">
<div class="column">
5

</div>
</div>
</div>
<div class="page" title="Page 6">
<div class="layoutArea">
<div class="column">
Figure 2: This figure illustrates all the MW disk particles (in blue) from the data you are using (projected on the x-y plane). Here we choose the disk particle type as an example. Following the instructions in Step 1, you need to call COMdefine to find a first estimate for the COM position vector (the red point) using all the particles, and then find the farthest particle (pointed by the cyan arrow) with respect to the estimated COM position. All the particles within half the length of the cyan arrow in the estimated COM frame (inside the green circle) will be utilized later to refine the COM calculations. Again, note that this picture is in 2D, but your data is in 3D and you should calculate all stuff in 3D.

</div>
</div>
<div class="layoutArea">
<div class="column">
6

</div>
</div>
</div>
<div class="page" title="Page 7">
<div class="layoutArea">
<div class="column">
Figure 3: This figure illustrates the next step to refine the COM calculations. In this figure, only the particles within the green circle (as in Fig. 2) are shown. Also, all particles are drawn in the frame of the first COM guess (the red point). Following the instructions in Step 2, you need to call COMdefine to find the 2nd guess of the COM (as denoted by the green point) using all the particles inside this green circles, and then quantify the change in COM position between two guesses (as denoted by the magenta arrow)). If the magnitude of the change vector is larger than the input tolerance (delta), then you need to perform such refinement steps again and again until the magnitude of the change vector is smaller than the input tolerance (delta). For example, the orange circle (whose radius is half the radius of the green circle) indicates where you should perform the 3rd guess.

</div>
</div>
<div class="layoutArea">
<div class="column">
7

</div>
</div>
</div>
<div class="page" title="Page 8">
<div class="layoutArea">
<div class="column">
3. 4.

7

• •

•

</div>
<div class="column">
What is the magnitude of the current separation (in kpc) and velocity (in km/s) between M33 and M31? Round your answers to three decimal places.

Given that M31 and the MW are about to merge, why is the iterative process to determine the COM is important?

Homework Submission

You must DOCUMENT your code. Explain each step.

Create a directory called Homework4. Save your code and answers to section 6 in that

directory. Your answers to section 6 should be saved EITHER: 1. As part of your Jupyter notebook solution.

2. Take a screen shot of your python output (with the relevant print statements for each quantity) from the command line.

Upload your Homework4 directory to your public 400B yourlastname repository on GitHub

</div>
</div>
<div class="layoutArea">
<div class="column">
8

</div>
</div>
</div>
