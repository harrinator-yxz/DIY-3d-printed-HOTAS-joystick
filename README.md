# DIY-3d-printed-HOTAS-joystick
## What is this repositiory for?
this repo is for notes and files to help built a diy fully 3d printed HOTAS joystick that uses STM32 and hid. it will include files along with some instructions links, pictures and software to help you along your journey.

## Getting started.

To get started I will show and talk about some of the main componetns and parts of the joystick including the gimbal, grip and electronics. <br>
### Grip
The stick/grip that I will be using is the [F-16 Sidestick Grip](https://www.printables.com/model/233472-f-16-sidestick-grip) By [Spock](https://www.printables.com/@Spock) On [printables.com](Printables) I found that it is one of the better free joystick grips. little to no supports and lots of customization options for multiple way switches, buttons, and potentiometers. Some of the buttons even have the ability to be 5 way switches, that is left, right up, down, and in. 
### Gimbal
The next big part is the gimabl, is am using is the [Real Robots Modular Joystick](https://www.thingiverse.com/thing:4732811) which is a big modular kit with some great stuff. You can check out the real robots kickstarter where you can buy a full kit with throttle and other code [here](https://www.kickstarter.com/projects/realrobots/real-robots-game-controller-construction-kits) But I will not be using any of this other than the gimbal from the joystick base as it is one of the cheaper easier to build gimbals aviable. it also has very few parts and is extremly staight forward to build.

### Electronics.
For my joystick I used an STM32F103C8T6 dev kit board, I would recommend buying one from a trusted source on Aliexpress or Digikey. However if you are tight on budget, then I found the Chineses CS32 f103 to be the best fake stm32. These CS32's are all over places like Temu and Aliexpress. I bought two different ones from temu, One was alright and could take the code/software, and the other could not hold the high baud rate. The fake chips do tend to have extremly bad ADC's which is neccacary for this as we will be using multiple buttons and potentiometers. The bad ADC's on the fake chips tend to have lots of noise, mine even had crosstalk between ADC channels.

> ### **why use an STM32?**
