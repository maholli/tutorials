
# Cutting PCB Stencils from Polyimide 
## A guide for the lab64 trotec laser cutter

This write-up documents a working procedure for cutting PCB stencils on the trotec 130W CO2 laser cutter. 
This procedure is **by no means** optimized and users are encouraged to experiment with better methods/techniques. 

The thickness of the stencil and the size of the openings are specific for each component included in the PCB design and will be defined by the manufacturer (typically in the datasheet). This tutorial describes a process for cutting a non-adhesive polyimide (aka Kapton) film that is 0.005 inch (5 mils) thick. 



<p align="middle">
  <img width="700" src="https://github.com/maholli/lab64/blob/master/pcb/stencils/images/1.PNG">
</p>

1.	Begin by exporting the solderpaste artwork from the PCB layout tool. This example shows the process for Autodesk's Eagle layout software. The relevant layers in Eagle are shown above.
	>NOTE: although we won't be cutting the board outline, it's important to include for scaling/alignment purposes. 

<p align="middle">
	<img width="500" src="https://github.com/maholli/lab64/blob/master/pcb/stencils/images/2.PNG">
</p>
	

2.	After configuring the layers, the artwork must then be exported in SVG format. Eagle does not have a native SVG exporting feature, so [download this Eagle ULP script](https://github.com/maholli/lab64/blob/master/pcb/stencils/eagle2svg-1_4_1.ulp). Once downloaded, click FILE -> Run ULP -> Browse -> and choose the downloaded script. Setup the export window as shown.

<p align="middle">
  <img width="700" src="https://github.com/maholli/lab64/blob/master/pcb/stencils/images/3.PNG">
</p>

3.	Once exported, open the SVG file in Inkscape. This can be done on the laptop in 004 if you don't have Inscape installed.

4.	Begin preparing the SVG file by selecting everything (Ctrl+A on windows), then ungroup everything (Ctrl+U) This will maintain each component's group, but allow the PCB outline to be selected.

5.	Select each piece of the board's outline by left clicking and holding shift. Ensure you've selected corners that have a radius and any other small features along the line.

6.	With the entire boarder selected, group the outline paths together (Ctrl+G)

<p align="middle">
  <img width="250" src="https://github.com/maholli/lab64/blob/master/pcb/stencils/images/4a.PNG">
</p>

7.	The Fill and Stroke parameters of the group will now be undefined (the highlighted question mark in the image above). 
	>NOTE: If you do not seen the Fill and Stroke menu, enable it by going to EDIT -> Fill and Stroke (Shift + Ctrl + F). 

<p align="middle">
  <img width="250" src="https://github.com/maholli/lab64/blob/master/pcb/stencils/images/4b.PNG">
</p>

8. While on the Fill tab, click the "X" box to change the paint parameters from "undefined" to "no paint."

9.	Next, with the border still selected, go to the stroke paint tab and change the RGB value from pure black to pure blue (RGB values of R: 0, G: 0, B: 255, A: 255).

<p align="middle">
  <img width="700" src="https://github.com/maholli/lab64/blob/master/pcb/stencils/images/5.PNG">
</p>

10.	For the trotec, it's important your stencil design doesn't contain any lines (or edges) that run parallel to the axis of movement. Therefore, select the entire design again (Ctrl +A), and left click once on any line in your design to change the bounding-box from "transform" mode to "rotation" mode. Hover your mouse above one of the small white boxes located at the corners of your design. The cursor should change into a rotation symbol. While still holding Ctrl, click and drag the mouse to the left in order to rotate the design 45 degrees. Unless your board contains components at odd angles, your design should now look similar to the design above.
	>NOTE: Many of the footprints have been removed from the design in shown above to allow for soldering of only a portion of the board. 

11.	After rotating, the design is now larger than the Inkscape canvas. To fix this, go to FILE -> Document Properties (Shift + Ctrl + D) and increase the Width and Height values to exceed the blue board outline by about at least 0.5 inch. 

12.	Close the Document Properties windows (**NOT the main Inkscape window**) and position the design in the middle of the canvas by selecting all (Ctrl + A) and left-click dragging.

<p align="middle">
  <img width="700" src="https://github.com/maholli/lab64/blob/master/pcb/stencils/images/6.PNG">
</p>

13. Save the Inkscape design as a **Plain SVG**.

14.	If it isn't already, move the plain SVG file to the 004 laptop via USB flashdrive.

15. After opening the plain SVG, send the design to the trotec laser by going to File -> Print (Ctrl + P).

<p align="middle">
  <img width="700" src="https://github.com/maholli/lab64/blob/master/pcb/stencils/images/7.PNG">
</p>

16.	Ensure the trotec engraver is selected in the print dialog and click "Preferences," and configure the trotec window as shown. 
	>NOTE: in this case, it's very important that Resolution is set to 1000 dpi.

17.	If the trotec software ("JobControl") wasn't already running, it will be started and appear along the bottom windows taskbar. 
	>NOTE: for designs with lots of components or features, the trotec print drivers may take up to 10 minutes to parse the file. Be patient! 

18. While the file is being parsed, start the trotec chiller and then turn on the laser cutter.

	### Film Preparation

<p align="middle">
  <img width="700" src="https://github.com/maholli/lab64/blob/master/pcb/stencils/images/9.jpg">
</p>

19.	Keeping in mind the size of your stencil and being conscientious of the cost of polyimide, use a straight edge to cut an appropriate sheet from the roll.

<p align="middle">
  <img width="700" src="https://github.com/maholli/lab64/blob/master/pcb/stencils/images/10.jpg">
</p>

20.	Use the contact-tape to cover the polyimide sheet and adhere it to a flat piece of Duron scrap. Ensure there is uniform contact across the film. Squeegee out any bubbles if necessary.

<p align="middle">
  <img width="700" src="https://github.com/maholli/lab64/blob/master/pcb/stencils/images/11.jpg">
</p>

21.	Position the Duron on the cutting-bed and focus the laser to the top of the contact-paper above the polyimide. Remember that the stencil design was rotated 45 degrees.

<p align="middle">
  <img width="700" src="https://github.com/maholli/lab64/blob/master/pcb/stencils/images/8c.PNG">
</p>

22. In the JobControl software, drag your design from the queue onto the honeycomb cutting area. Work back-and-forth between laser cutter and the laptop to ensure your design is aligned properly over the film. This can be tricky!

<p align="middle">
  <img width="700" src="https://github.com/maholli/lab64/blob/master/pcb/stencils/images/8b.PNG">
</p>

23. After the design is properly aligned, double click anywhere on the honeycomb (not on your design) and configure the laser parameters according to the image above. 

<p align="middle">
  <img width="700" src="https://github.com/maholli/lab64/blob/master/pcb/stencils/images/12.jpg">
</p>

24. Double check you did not skip a step before starting the job. Let all three passes complete (even though it looks like it isn't necessary, the three passes are needed for small detailed pads). As shown above, debris from the Duron will collect above the design.

25. After the laser is finished, gently brush the debris off the contact-paper with a dry paper towel before peeling the stencil off of the Duron. 

<p align="middle">
  <img width="700" src="https://github.com/maholli/lab64/blob/master/pcb/stencils/images/13.jpg">
</p>

26. Some Duron compositions are better than others for this process. As you can see, there will be cutting residue on the bottom side of the stencil. Use a paper towel with isopropyl alcohol to remove the residue.

<p align="middle">
  <img width="700" src="https://github.com/maholli/lab64/blob/master/pcb/stencils/images/14.jpg">
</p>

27. Carefully remove the contact-paper from the topside and continue cleaning with isopropyl alcohol. A freshly cut stencil that's been (mostly) cleaned is pictured above. 

### Congratulations! You made your first stencil. I'll work on adding a section to this write-up detailing how I like to stencil solderpaste onto a board. Here's an example of what that'd look like:

<p align="middle">
  <img width="700" src="https://github.com/maholli/lab64/blob/master/pcb/stencils/images/16.jpg">
</p>


