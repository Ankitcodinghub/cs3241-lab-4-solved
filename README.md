# cs3241-lab-4-solved
**TO GET THIS SOLUTION VISIT:** [CS3241 Lab 4 Solved](https://www.ankitcodinghub.com/product/cs3241-solved-12/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;126911&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CS3241 Lab 4  Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

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

<div class="kksr-stars-active" style="width: 138px;">
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
            5/5 - (1 vote)    </div>
    </div>
LEARNING OBJECTIVES

Implementing the Whitted Ray Tracing algorithm. After completing the programming assignment, you should have learned

• how to compute ray intersection with some simple implicit-form surface primitive,

• how to do lighting computation,

• how to shoot shadow rays to generate shadows,

• how to spawn secondary rays,

• how to trace rays recursively, and

• how the Whitted Ray Tracing algorithm works.

TASKS

You are to complete an incomplete C++ program that implements the Whitted Ray Tracing algorithm. You have to complete the program according to the following requirements. There are altogether three tasks in the assignment.

From the Canvas &gt; CS3241 &gt; Files &gt; Lab Assignments folder, download the ZIP file Lab4_todo_(*).zip.

It shows an image of an unlit scene of 3 intersecting planes and a cube made of triangles. Two additional spheres are supposed to be in the image, but the ray-sphere intersection routine has not been implemented yet.

Task 1

You are to complete the Sphere::hit() and Sphere::shadowHit() functions in Sphere.cpp to compute ray-sphere intersection. You must write your code only in places marked “WRITE YOUR CODE HERE”.

You can refer to Plane.{h, cpp} and Triangle.{h, cpp} to get some idea how to do it. Other relevant files to study are Vector3d.h, Ray.h, Surface.h, and Sphere.h.

For this task, you have to submit your completed Sphere.cpp, and the image generated, which should look like the following. You must name your image file img_spheres.png.

img_spheres.png

Task 2

You are to complete the Raytrace::TraceRay() function in Raytrace.cpp to perform the recursive ray tracing. You must write your code only in places marked “WRITE YOUR CODE HERE”.

In this implementation, we are assuming that all objects are opaque. At each surface point intersected by the ray, the color result is computed using the formula

𝐼 = 𝐼𝑙𝑜𝑐𝑎𝑙 + 𝑘𝑟𝑔 𝐼𝑟𝑒𝑓𝑙𝑒𝑐𝑡𝑒𝑑

where

𝑀

𝐼𝑙𝑜𝑐𝑎𝑙 = 𝐼𝑎𝑘𝑎 + ∑ 𝑘𝑖,𝑠ℎ𝑎𝑑𝑜𝑤 𝐼𝑖,𝑠𝑜𝑢𝑟𝑐𝑒[𝑘𝑑(𝑵 ∙ 𝑳𝑖) + 𝑘𝑟(𝑹𝑖 ∙ 𝑽)𝑛] 𝑖=1

and M is the number of point light sources in the scene.

The relevant files to study first are Vector3d.h, Color.h, Ray.h, Material.h, Light.h, Surface.h, Scene.h and Raytrace.h.

For this task, you have to submit your completed Raytrace.cpp, and the images generated by the program, which should look like the followings. There are 6 images you need to submit, and you must name them as shown at the bottom of each image shown below.

img_r0.png

reflectLevels = 0 hasShadow = false img_r0s.png

reflectLevels = 0 hasShadow = true

img_r1.png

reflectLevels = 1 hasShadow = false img_r1s.png

reflectLevels = 1 hasShadow = true

img_r2.png img_r2s.png

reflectLevels = 2 reflectLevels = 2

hasShadow = false hasShadow = true

Each of these images should take less than 10 seconds to produce. On my laptop, img_r2s.png (the most time-consuming) took about 1 second. In your IDE (e.g. Microsoft Visual Studio, Xcode), make sure you compile your program using the Release configuration.

Task 3

You are to complete the DefineScene2() function in Main.cpp to model a new scene for rendering. You must write your code only in places marked “WRITE YOUR CODE HERE”.

You must use all the surface primitive types, namely, plane, sphere, and triangle, in your scene model. This task will be assessed based on the fulfillment of the above basic requirements, on the technical difficulty and object’s complexity, and on the aesthetics and creativity. Your scene model should be rendered with reflectLevels=2 and hasShadow=true, and an image resolution of 640×480. Name your image file img_scene2.png.

For this task, you have to submit your completed Main.cpp, and the generated image img_scene2.png.

GRADING

Good coding style. Comment your code adequately, use meaningful names for functions and variables, and indent your code properly. You must fill in your name, and NUS User ID in the header comment.

SUBMISSION

For this assignment, you need to submit only the following 11 files:

• Sphere.cpp and img_spheres.png,

• Raytrace.cpp and img_r0.png, img_r0s.png, img_r1.png, img_r1s.png, img_r2.png, img_r2s.png,

• Main.cpp and img_scene2.png.

You must put it/them in a ZIP file and name your ZIP file nus-user-id_lab4.zip. For example, if your NUS User ID is e0123456, you should name your file e0123456_lab4.zip.

Note that you will be penalized for submitting non-required files.

——— End of Document ———
