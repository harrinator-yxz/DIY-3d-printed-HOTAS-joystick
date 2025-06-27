---
title: DIY 3d printed HOTAS
author: Harry Connolly (harrinator-yxz)
description: a full guide on how to fully create, 3D print, and assemble a whole HOTAS setup.
created_at: 2024-03-20
---




### June 8th: Project startup

I started this project by just looking for some files and resources to get started.
I found:

- The [Olukelo gimbal](https://www.thingiverse.com/thing:2496028)
- The [Real Robots Modular Joystick](https://www.thingiverse.com/thing:4732811)
- [F-16 Sidestick Grip](https://www.printables.com/model/233472-f-16-sidestick-grip) By [Spock](https://www.printables.com/@Spock) On [printables.com](Printables)
- [Freejoy](https://github.com/FreeJoy-Team/FreeJoy)
  

along with multiple other videos about DIY Hotas's and even a [Reddit Page](https://www.reddit.com/r/HotasDIY/)




**Total time spent: 4h**

### June 10th: Deciding on parts

I decided to use the [Real Robots Modular Joystick](https://www.thingiverse.com/thing:4732811) For my Gimbal. I also decided to slighly modify this for my purpose and for easier recreation.
The first modification was creating a hole through the joystick stick that connects all the mechanical proccess to the stick above There is already

<img src="/Images/stick.png" alt="stick" width="200" />
<img src="/Images/Springhammer1.png" alt="stick" width="200" />

**Total  time spend: 3h**


### June 11th: parts

I spent today just deciding what parts to use. For the buttons I was looking at 7mm momentary push buttons. I just decided on these because I couldnt be bothered finding 5 way or 4 way buttons. Also I ordered these just from temu just because they were cheap lol.    I spent most of today downloading and installing 



### June 19th;  Multiple days work 

AFter printing the gimbal i found many flaws but i stuck with it and for the next week I tryed to get it working, after it braking wiht just 2 practice movements i knew something had to be changed.I 3d printed a smaller test version of the gimbal and I did not like the feel, and it was extremly limited and bad. It also used two potentiometers which were not even able to be read properlly due to the ADC's on my test raspberry pi pico not being ableto handle the two inputs which cross talk and lots of noise.

Today i have started designing my own gimbal. The plan for this is:
 - 3 Axis - with twist rudder controls:
 - easy to assemble
 - Cheap
 - Hall effect sensors for greater accuracy.
 - few parts.
 - easy configurable code/HID

So far I only have the first axis done. IT uses 688zz ball bearings along with a simple design. I am hoping to build on this adding multiple other life featurs



<img src="/Images/first axis.png" alt="stick" width="500" />

***Total time spent last few days: 7h***


### June20th; Deciding on readings

I decided to use halle ffect sensors, i spent most of today just designing how I was going to mount them to the gimbal. The way i have come up with allows for adustment and easy maintenecce. I also imported the f16 sidestick grip as a refrence by spock. I hope to get the second axis done by the end of the week.

<img src="/Images/RENDER.PNG" alt="render" width="700" />

**Total time: 2 hours**

### June22nd: 2nd Axis completed

I started today by prepping thee gimbal for a 2nd axis, doingthings like adjusting sizes to how big i want it to be irl, and deciding which bearings to use (688zz ball bearings) then i modeled the 2nd axis, which was quite easy because I just did it trhe same as the first. The luttle L shaped pieces are going to have magnets either side and the hall effect sensor in the middle which is how i will get my readings. I also added screw holes to cerrtain places that nedded them and tommorow I am going to try and prep the model for a test, by adjust things aadding scre holes and finalising. Then I will start the twist rudder controlls. I also decided to go with a circular base, just because I think it looks cool.
<img src="/Images/gimbal v9.png" alt="render" width="700" />


**total time: 4h**

### June 23rd: SMALLER!!

I spent today making it smaller as ther was lots of unnescacary space, I have noew reduced the outside circle diameter to 165mm which is much more bareable than the 230mm it was befroe. I also Added screw holes in different places, as I had to cut up some pieces so I can assemble it, I also added joints in Fusion and simulated the 2 degrees of freedom which worked quite nicely ( although sdtrasining my pc)  I have left enoug room for 20 degrees of rotation in each axis (+/-) so 20 degrees forward and 20 back so 40 in total, I decided on 20 because thats what the Thrustmaster Warthog uses and I am trying to base this off that.

<img src="/Images/gimbalv10.jpg" alt="render" width="700" />

**Total time: 1 hour**

### June 24 - 27th

Not much happened on the 24th and 25th but today and yesterday I have been hard at work working on he twist ruddeer controlls. After some consideration, I decided on a small form simple design. The little raft in the middle holds 2 springs, one on either side, and when you rotate it it compresses one of the springs, applying tension and force back. The little holes on the opposite side are just palceholders at the moment, as I kind of need to print this and test before I decideo on how I am going to mount the magnets and Hall sensors, Right now the general consessis is to mount the Hall effect sensor throug hthe little hole and have the magnets rotate around it. It turns out that calculating distances between circles and all that is much harder than what i can handle because its pretty much calculus and triganomitry.

<img src="/Images/Twist Controlls v1img.png" alt="render" width="400" />
<img src="/Images/twist.gif" alt="render" width="400" />

**Time spent 3 hours**



