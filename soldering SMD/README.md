# Soldering Surface Mount Devices (SMD)

A brief primer on surface mount soldering to aid in lab64 SMD soldering exercises.

## Table of Contents  
[SMD Soldering in 6 Easy Steps](#smd-soldering-in-6-easy-steps)<br>
[Know your tools](#know-your-tools)<br>
[Detailed lab64 SMD Soldering Procedure](#detailed-lab64-procedure)<br>
[SMD Soldering by Hand](#smd-soldering-by-hand)<br>

<br><img width="800" src="https://github.com/maholli/tutorials/blob/master/soldering%20SMD/images/9bbb.jpg"><br>

Every aspect of surface mount soldering was engineered to make large-scale PCB assembly faster and more reliable. With proper setup and execution, everyone can enjoy the benefits of SMD soldering on their projects!

## SMD Soldering in 6 Easy Steps
1. Mount PCB in fixture
2. Align solder paste stencil
3. Squeegee solder paste over stencil
4. Carefully remove stencil
5. Place components
6. Reflow inside pre-configured SMD reflow oven

> But don't let the small amount of steps fool you, SMD soldering can be tricky if not approached correctly. We'll continue the tutorial by first introducing the tools before going through each step in more detail.

## Know Your Tools
* **Solder Paste** SMD soldering uses solder paste to form the electrical connections. Solder paste is almost like *powdered* metal solder suspended inside a high-viscosity flux. The goal of SMD soldering is to prepare each pad on the PCB with a *just* the right amount of solder paste which can then melt and bond to the component leads. <br><img width="400" src="https://github.com/maholli/tutorials/blob/master/soldering%20SMD/images/1.jpg"><img width="400" src="https://github.com/maholli/tutorials/blob/master/soldering%20SMD/images/6.gif"><br><br>
* **Solder Stencil** Usually ~0.005 inches thick of either stainless steel or polyimide (Kapton) sheet with precise apertures cut for each footprint on the PCB. <br><img width="400" src="https://github.com/maholli/tutorials/blob/master/soldering%20SMD/images/osh1.jpg"><img width="400" src="https://github.com/maholli/tutorials/blob/master/soldering%20SMD/images/osh2.jpg"><br>image courtesy of OSHstencils <br><br>
* **Squeegee** A tool used to pushed solder paste into the holes of the stencil. A squeegee's thickness and flat edge play a big role in the successfulness of the stenciling process. We use modified putty knifes in lab64, but there are many other (better) options. <br><img width="400" src="https://github.com/maholli/tutorials/blob/master/soldering%20SMD/images/10.jpg"><br><br>
* **Mounting Fixture** Probably the most difficult part of solder stencil work is figuring out how to hold the PCB and stencil. The successfulness of your stencil job relies on the planarity between the board and your stencil! In the lab64 tutorial, we have built a nice fixture to make things go smoothly. However, when trying this on your own, it's common to hold the PCB and stencil like this: <br><img width="400" src="https://github.com/maholli/tutorials/blob/master/soldering%20SMD/images/osh5.jpg"><img width="400" src="https://github.com/maholli/tutorials/blob/master/soldering%20SMD/images/osh6.jpg"><br>image courtesy of OSHstencils <br><br>

# Detailed lab64 Procedure
1. This exercise uses a PCB mounting fixture. Although the fixture won't look exactly like the clip below, the first step of our SMD soldering tutorial will involve carefully placing the PCB inside the fixture.<br><img width="800" src="https://github.com/maholli/tutorials/blob/master/soldering%20SMD/images/5.gif"><br>clip courtesy of <br><br>
2. Next, it's important to make any necessary tweaks and adjustments to the PCB position as well as the stencil location to ensure good alignment over the pads. This takes practice, but is key to successful stencil work. Be mindful of the planarity between the PCB and the stencil. Is the stencil bowed? <br><br>
3. The time has come to apply paste! Begin by applying a generous amount of solder paste to the squeegee as shown in the clip below. Then, place the squeegee at ~45 degrees to the stencil and begin slowly pulling it back towards your body. Don't be afraid to apply pressure with the squeegee, but DO try and limit the number of passes you make over the entire stencil, since each time you lift and repeat the process, you run the risk of moving the stencil and causing paste to leak out from the apertures.<br><img width="800" src="https://github.com/maholli/tutorials/blob/master/soldering%20SMD/images/9bb.gif"><br>clip courtesy of <br>notice how the operator changes the angle of his squeegee at the end of the process to shear the remaining paste away from the stencil.<br><br> 
4. After applying paste to your board, it's necessary to remove the stencil without disrupting the small islands of solder you've worked so hard to create. After removing the stencil, the solder paste should look like this: <br><img width="800" src="https://github.com/maholli/tutorials/blob/master/soldering%20SMD/images/2.jpg"><br><br>
5. With paste on the board, it's now time to place components. Tweezers are a must (clean the tips for reduced frustration on smaller parts). Try not to make adjustments once the part is placed since this usually results in more work than it saved. Make sure you're placing the correct components in each spot! It's easier to double-check the reference designator now than to rework the board later.<br><img width="800" src="https://github.com/maholli/tutorials/blob/master/soldering%20SMD/images/3.gif"><br>clip courtesy of <br><br>
6. Almost there! Now that all the parts are placed, it's time to heat the board inside a reflow oven. Be mindful of the temperature profile programmed in to the oven. In lab64, all the solder paste is lead-free, so the ovens are programmed accordingly and won't work as well for leaded solders (without changing the profile). The wonderful part about SMD soldering is the "restoring force" of surface tension. As shown below, surface tension of the molten solder causes components to align themselves! <br><img width="800" src="https://github.com/maholli/tutorials/blob/master/soldering%20SMD/images/4.gif"><br>clip courtesy of <br><br>
* **PCB Cleaning?** Most solder pastes use a "no clean" flux which is designed to remain on the board after reflow. However, this isn't always the case. Check the solder paste you're using and make sure to wash (and thoroughly dry!) the board afterwards, if necessary, to prevent corrosion. <br><br>
* **Workspace Cleaning** Don't leave a mess for others! Carefully return any unused solder paste on your squeegee back into the container from which it came. Wipe down your work surface with a IPA and a paper towel.
>**Anything that has solder on it must not go in the trash!! Place used paper towels, toothpicks, etc... in one of the many label Solder Waste Disposal bins.**   

## SMD Soldering by Hand
SMD soldering can still be beneficial, even if you don't have a stencil or reflow oven. Below are some tips/techniques to try in your own lab.<br><br>
* **Hand Soldering SMD Components** Although not designed for hand soldering, most SMD components are manageable with a soldering iron and a steady hand. There are different techniques for different packages. Below is my preferred method of soldering small passive components. Using smaller gauge solder wire when working with SMD components is helpful in avoiding excessively large solder joints. <br><img width="800" src="https://github.com/maholli/tutorials/blob/master/soldering%20SMD/images/9.gif"><br>clip courtesy of <br><br>
* **Hand-dispensing Solder Paste** Although stencils make quick work of paste dispensing, it can also be done by hand. Using either a toothpick-like tool or the syringe tip (if purchased with your paste), apply a small amount to each pad like so: <br><img width="800" src="https://github.com/maholli/tutorials/blob/master/soldering%20SMD/images/7.gif"><br>clip courtesy of <br><br>
* **Hot Air Tools** There are a multitude of hot air soldering/rework tools on the market. Below is a clip illustrating how heat, flux, and surface tension can "magically" solder the leads of a quad-flat pack (QFP) with very little bridging (and shows how to fix when bridges do occur): <br><img width="800" src="https://github.com/maholli/tutorials/blob/master/soldering%20SMD/images/9b.gif"><br>clip courtesy of <br><br>
