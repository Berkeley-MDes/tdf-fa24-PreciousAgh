# Hello DES INV 202 Student!
Welcome to your new GitHub repository! 

# Outline
[week 1](README.md#week-1-example-report-1)

week 2, etc...

---

# Github Background Information & Context
If you’re new to GitHub, you can think of this as a shared file space (like a Google Drive folder, or a like a USB drive that’s hosted online.) 

This is your space to store project files, videos, PDFs, notes, images, etc., and (hopefully, neatly) organize so it's easy for viewers (and you!) to navigate. That said, it’s super easy for you to share any file or folder with us (your TDF instructional team) - just send us the link!  As a start, feel free to simply add images to the `/assets` folder, which is located [here](/assets). 

The specific file that I’m typing into right now is the **README.md** for this repo. 
##### (💡 TIP: The .md indicates that we’re using [Markdown formatting.](https://www.markdownguide.org/cheat-sheet/)) #####
<h6> (💡 TIP 2: GitHub Markdown supports <a href="https://gist.github.com/seanh/13a93686bf4c2cb16e658b3cf96807f2"> <em>HTML formatting</em> too, including emojis 😄</a>, in case that helps!) </h6>

### :star: Whatever you write in your **README.md** will show up on the “front page” of your GitHub repo. This is where we’ll be looking for your [weekly progress reports](https://github.com/Berkeley-MDes/24f-desinv-202/wiki/3.0-Weekly-Submissions#weekly-progress-report). They might look something like this: ###

# Week 1 #
## Week of 09/05/2024

This week I learnt how to laser cut and Design on Adobe Illustrator

**Project Idea:** I initially designed a wooden flower, which I later decided to convert into a coaster decor by adding squares to the design.

**Key Learnings:**
1. Adobe Illustrator Skills:
   I learned how to design intricate patterns and adjust shapes to fit the laser cutter's capabilities.
2. Laser Cutting Process:
   - Gained experience with using the laser cutter, especially understanding how different line thicknesses affect cutting time.
   - The original design had thick lines, causing the cutting process to take up to 2 hours.
   - By adjusting to thinner lines, I reduced the cutting time significantly to just 12 minutes.

My Work
---

<img width="200" alt="flowerlasercut" src="assets/IMG_1175.jpeg">, <img width="200" alt="flowerlasercut" src="assets/IMG_1178.jpeg">, <img width="200" alt="flowerlasercut" src="assets/IMG_1180.jpeg">

---

**Challenges:**
    The initial coaster was too large, and I had to make design adjustments for efficiency.
    
**Next Steps:**
Plan to reuse the leftover wood from the coaster project to create a wooden keychain.

**Next week plans**
- Continue learning tutorials on Rhino


---

# Week 2 # 

This week, I focused on experimenting with the existing cellphone stand file in Grasshopper, created my own rhino file and created a shape on grasshopper. Here’s a summary of my progress and observations:

---

## Experimenting with the Existing Cellphone Stand Design ## 

**Baking the Existing 3D Model:**
I began by baking the current cellphone stand design to visualize the 3D image. 

<img width="500" alt="rhino" src="assets/Image 1.png">

**Sphere Radius Adjustments:**
I then experimented with the sphere radius, initially set between 40 to 50 units. I extended the radius to 61 units to observe how this affected the overall design.


<img width="500" alt="rhino" src="assets/Image2.png">


**Fit Issues with Increased Sphere Size**
When the sphere radius reached 61 units, I noticed that it was too large for the phone fitting, leading to a red warning indicating that the design would not fit the phone properly. (Insert an image showing the warning or red indicator in Grasshopper here to emphasize the fit issue.) This observation suggests that there is a set limit for the design to ensure the proper fitting of the phone. I am currently looking for the specific parameter that controls this limit.

<img width="500" alt="flowerlasercut" src="assets/Image3.png">


**Exploring the Cellphone Stand Cluster**

To find the fitting limit, I navigated to the cellphone stand cluster, which manages key design parameters like the phone width in millimeters. This setting ensures the phone fits correctly in the stand.

<img width="500" alt="flowerlasercut" src="assets/image4.1.png">

By double-clicking on the cluster, I accessed its internal components, where I found detailed controls for adjusting dimensions like the phone width. This allowed me to experiment with different values to achieve a better fit for the phone. 

<img width="500" alt="flowerlasercut" src="assets/image4.2.png">

 
**Experimenting with Shape Changes**
I also experimented with altering the shape of the cellphone stand, attempting to change the design from two spheres to one box. However, I decided to move on from this experiment as the design wasn’t progressing as expected.

<img width="500" alt="flowerlasercut" src="assets/Image 5.png">

## Creating a Trifold Phone Stand in Rhino##
**Objective:**
To design a trifold phone stand using basic tools in Rhino, including creating and positioning solid shapes with precision.


**Creating a Rectangle:**

I started by creating a rectangle in Rhino, which served as the base component for the phone stand.
**Viewing in Shaded Mode:**

To better visualize the design, I switched to Shaded mode in the viewport. This provided a clearer view of the solid shapes as I built the phone stand.

<img width="500" alt="flowerlasercut" src="assets/rhinoimage1.png">



**Using Gumball for Adjustments:**

I utilized the Gumball tool to make precise adjustments to the position and slant of the supporting parts. This allowed me to rotate and move the pieces, giving the stand its distinctive slanted support to hold a phone at a convenient viewing angle.


<img width="500" alt="flowerlasercut" src="assets/rhinoimg3.png">


**Final Phone stand**

Here is the final trifold stand


<img width="500" alt="flowerlasercut" src="assets/rhinofinal.png">


**Next Steps:**
Refining the fit and making any necessary adjustments to the design for stability. Everthing was just manually designed without further customization.

---


## Creating an Object on Grasshopper ## 


**Objective:** To design a stacked structure consisting of a curved triangle, a circle, and another triangle using Grasshopper.

**Step 1: Creating the Curved Triangle**

To create the design, I started by making a curved triangle using the Polygon component, where I set the radius, segments, and fillet radius to achieve the desired shape. Afterward, I extruded the triangle by connecting the polygon to an Extrude component, setting the direction using a Unit Z vector, and controlling the extrusion depth with a Number Slider. I then connected the radius factor to the Unit Z vector and added a Cap component to close the top and bottom, forming a solid triangle polygon.

<img width="500" alt="grasshopper" src="assets/grasshopper1.png">


**Step 2: Adding the Circle**

Next, I moved on to adding a circle above the triangle. I created a circle and set its radius with a Number Slider, then used a Move component to position it above the first triangle, moving it along the Z-axis with a Unit Z vector. I connected the circle to the Move component and extruded it, again controlling the depth with a Number Slider. To finalize, I applied a Cap component to close the extruded circle.

<img width="500" alt="rhino" src="assets/grasshopper 2.png">


**Step 3: Repeating for the Top Triangle**

Finally, I repeated the process from the first step to create another triangle. I moved this second triangle above the circle using the Move component, adjusting its position on the Z-axis with a Number Slider to place it properly. The top triangle was also capped to complete the design. This resulted in a stacked structure with a triangle on top of a circle, which was placed on top of another triangle, all fully extruded and capped.


<img width="500" alt="rhino" src="assets/grasshopper 3.png">

---


## Week 3 ##

# Project 1: Computational Design Progress Report

## Jewelry Stand Design with Grasshopper

### 1. Project Overview
This week, I started working on my computational design project for **Project 1**, where I designed a **jewelry stand** using **Grasshopper & Rhino**. I challenged myself by choosing the **Axolotl** level, which pushed me to explore complex geometries and transformations in Grasshopper.

### 2. Design Process

#### 2.1 Grasshopper File Explanation
In this project, I created a design composed of:
- **A polygon base**: The stand starts with a polygon shape that forms the base.
- **Cylinder and Polygon Structures**: I added a cylinder and another polygon on top. These shapes were moved, rotated, and extruded to create the overall stand structure.
- **Rotation Axis**: One of the key transformations was using the **rotate axis** tool, which allowed me to position parts of the design dynamically.


<img width="500" alt="rhino" src="assets/grasshopper 3.png">


#### 2.2 Printing and Challenges
When I initially printed the stand, I faced a challenge: the design came out flat and lacked the intended depth. To resolve this, I introduced a **hollow triangle** to support the design and give it the three-dimensional form it needed. This adjustment brought the entire structure to life as I had envisioned.


<img width="500" alt="rhino" src="assets/grasshopper 3.png">, <img width="500" alt="rhino" src="assets/grasshopper 3.png"> 
<img width="500" alt="rhino" src="assets/grasshopper 3.png">, <img width="500" alt="rhino" src="assets/grasshopper 3.png">


### 3. Reflections
I am proud of the progress I’ve made so far. This project challenged me to think critically about computational design and the tools I used. Solving the issue with the hollow triangle was a pivotal moment, and it taught me a lot about how small adjustments can completely transform a project.

<img width="500" alt="rhino" src="assets/grasshopper 3.png">

### 4. Video Demonstration
To see my full design process in action, watch the video below where I demonstrate the steps taken and how I refined the design over time. In the video, I also explain how I resolved key challenges and what I learned along the way.

[Watch the full video of my work](#) <!-- Add a link to the video here -->

---
Stay tuned for more updates on this project as I continue refining the design and tackling new challenges!


## Quick Links, compiled here for your convenience: ##

- [TDF Wiki](https://github.com/Berkeley-MDes/24f-desinv-202/wiki) - the ultimate source for truth and information about the course and assignments
- [Google Drive Folder](https://drive.google.com/drive/u/0/folders/1DJ1b6sSDwHXX6NRcQYt10ivyQSgU0ND6) - slides and other resources
- [bCourses](https://bcourses.berkeley.edu/courses/1537533) - where the grading happens
