# Soldering 101
Soldering is one of those skills that can be easy to learn, but hard to master. It's inherently simple, but unfortunately, **MANY** people find it difficult to solder and continue to struggle throughout their careers.
### With the amount of time EE and CS students will likely spend soldering, spending 5 minutes to read through this could save you countless frustrated hours at the bench. 

*This write-up is not comprehensive. Feedback is always appreciated: maholli@stanford.edu.*

## Table of Contents  
[Soldering crash course](#soldering-crash-course)<br>
[Important tips](#important-things-to-keep-in-mind)<br>
[Help! I'm still having trouble!](#i-am-still-having-trouble)<br>
[What is soldering?](#what-is-soldering)<br>
[What is solder?](#what-is-solder)<br>

## Soldering crash course
The goal of soldering is to make an electrical interconnect. Below is a very basic (but effective!) procedure.
1. Prepare and plan ahead! Secure your board, ensure you can reach the components in question, have all the tools you need nearby before starting.
1. Set the iron to an appropriate temp (750F for Pb-Free solder)
2. Remove the iron from the cradle and wipe the old solder from the tip using the gold-colored metal nest.
	> Train yourself to work deliberately, but quickly. The clock is ticking from the moment you remove the oxide layer from the tip.
3. Melt a small amount of solder onto the tip to ensure solder will "wet" (AKA stick) to the tip of the iron. 
4. Place the tip where you want the solder interconnect to form. Make sure you're making contact with BOTH the pad on the board and the lead of the component. This allows both surfaces to come up to temperature. You DON'T need to press hard!
5. Slowly feed solder into the joint. You may need to start by adding solder directly to the iron before there's enough flux to reduce the oxides on the surface of the component/board.
6. Remove the iron in one, deliberate, motion and then repeat!
7. After finishing your solder work, re-tin (melt a good amount of solder) onto the tip before returning it back to the cradle and turning off the iron.<br><br>Therefore, soldering a through-hole header pin using a flux-core solder should look like this...<br>
<img width="700" src="https://github.com/maholli/lab64/blob/master/soldering/images/2.gif"><br>clip courtesy of [Androkavo](https://www.youtube.com/watch?v=tfIwHuGzUEk)<br>
Watch the clip a few times and see if you can spot each step (#1-#6) listed above.

## Important things to keep in mind
1. Oxides are the enemy! If you've ever struggled to solder, or thought your iron wasn't getting hot enough, **it was probably due to oxide formation!** Oxide layers form on metal surfaces when exposed to oxygen in the air. They are **thermally insulating,** and they form faster at higher temperatures.<img width="700" src="https://github.com/maholli/lab64/blob/master/soldering/images/3.gif"><br>clip courtesy of [Androkavo](https://www.youtube.com/watch?v=tfIwHuGzUEk)<br><br> The clip above illustrates why flux is important. As you can see, the operator has pre-applied solder to the tip before making contact with the lead. As a result, there is no flux available to reduce the oxides present of the lead and pad. The result is a bad solder joint.<br><br> We could fix the soldering from the previous clip by using external flux. This is flux that we apply independently (as opposed to the flux-core solder wire which is our usual source of flux). Obviously you should avoid getting in this situation, but the clip below shows how helpful flux can be.<br><img width="700" src="https://github.com/maholli/lab64/blob/master/soldering/images/4.gif"><br>clip courtesy of [Androkavo](https://www.youtube.com/watch?v=tfIwHuGzUEk)<br><br> Note that the clip above is for illustrative purposes. It's best practice to reduce the number of times you let the board heat-up and cool-down (each heat/cool cycle degrades epoxy holding the PCB together).<br><br>The image below shows what soldering a surface mount lead looks like using external flux. Please note this method is different from using the flux-core solder wire since the operator has pre-applied solder to the tip. This technique should be considered when the previous method shown on the header pin is not possible.<br><img width="700" src="https://github.com/maholli/lab64/blob/master/soldering/images/5.gif"><br>clip courtesy of [Androkavo](https://www.youtube.com/watch?v=tfIwHuGzUEk)<br>
2. Most solder wire has a chemical inside called flux. Flux + heat breaks down oxides! You NEED flux to solder properly, but in most cases the flux inside the solder wire is enough. (P.S. flux is what causes the "fumes" you see while soldering)
3. **Your secret weapons while soldering are controlling/understanding heat flow, oxide formation, and surface tension.**
4. Size matters! Smaller soldering iron tips transfer heat slower than larger ones. Use the largest tip you can get away with and lower the tip temperature to achieve better control.<br><img width="900" src="https://github.com/maholli/lab64/blob/master/soldering/images/pic2.PNG"><br>image courtesy of [nasa technical standard: soldered electrical connections](https://nepp.nasa.gov/docuploads/06AA01BA-FC7E-4094-AE829CE371A7B05D/NASA-STD-8739.3.pdf)<br>
5. Think about HOW the heat is being transferred from the iron to your solder joint. Could there be something like an oxide layer or air gap between the tip and the pad that could be blocking the heat flow?<br><img width="700" src="https://github.com/maholli/lab64/blob/master/soldering/images/pic3.PNG"><br>image courtesy of [nasa technical standard: soldered electrical connections](https://nepp.nasa.gov/docuploads/06AA01BA-FC7E-4094-AE829CE371A7B05D/NASA-STD-8739.3.pdf)<br>
6. Increasing the iron temperature actually makes soldering HARDER! Expect for a few exceptions, increasing temperature is not going to fix any issues you may be having. For example:
	* Say you're having trouble melting solder onto the tip, and instead of using flux and the sponge to clean the tip, you decide to increase the temperature. Not only does this not fix the root cause, but the higher temperature will cause the oxide layer to grow even faster!
	* The higher the temperature, the faster the epoxy holding the PCB together will breakdown. This means it will be easier to lift pads or damage components from heat exposure.
		* EXCEPTIONS
			* It's acceptable to increase the soldering iron temperature when...
				* Switching from leaded to lead-free solder
					* For leaded solder, begin with the iron at 700F
					* For lead-free solder begin with the iron at 750F
			* if you're soldering something with a VERY large heatsink attached and you need a little extra "boost" of heat to help you soldering iron keep up with the heat loss. 

## I am still having trouble
Here are some common things to check when troubleshooting  a difficult soldering job:<br>
1. Solder doesn't stick to the soldering iron! It must be broken!<br><img width="700" src="https://github.com/maholli/lab64/blob/master/soldering/images/1.gif"><br>clip courtesy of [Androkavo](https://www.youtube.com/watch?v=JADI1N-K9Yc)<br>
	* Let's not jump to any conclusions, it's likely it was just used by an inexperienced operator that hasn't read this write-up yet. Wipe the tip off and see if solder will wet the surface. The solder should melt easily and stick to the iron. 
	* If the solder melts but doesn't stick, then your tip probably has a very thin oxide layer. Try again to melt some solder to the tip, then immediately wipe it off on the gold-colored metal sponge.  
	* If the solder doesn't melt easily, or you need to press hard in order to get it started, check the iron temperature and use a bit of tip-cleaner immediately before some aggressive cleaning.
2. How much metal is attached to the component/pad you're trying to solder to? Soldering to a large metal component or a ground/power plane is more difficult because it takes longer for the iron to heat that much mass. 
	* Use a larger tip (if possible). Be careful not to change the tip when it's hot!
	* Spend more time holding the iron to board/component before adding solder.
	* Try to solder the ground or power contacts one after another with minimal time between each other. This reduces the amount of heat you need to add back into the system and causes less damage to the board. 
3. Don't hold a component in place with metal tweezers/pliars! Adding that much thermal mass to the system will make it very hard to transfer enough heat to the joint. 
	* Place the component with tweezers, but use something like a wooden stick or plastic "spudger" to hold it in place while soldering.
4. Removing solder bridges across leads/pads.
	* Good use of flux and a clean tip makes removing solder bridges easy! The trick is coaxing the solder to stick to to the iron and/or adjacent pins.
	* Begin by applying paste flux to the target area as well as the surrounding leads. Make sure your tip is clean and then melt the smallest amount of solder onto the tip as you can. Place the iron across the bridge, ensuring you're making contact with at least the two target leads but ideally one or two adjacent leads as well. Pause for a moment to allow heat to equilibrate across the solder/leads. Without applying force (AKA very lightly) "drag" the tip away from where the original bridge location. "Away" could mean along the length of the leads and away from the package, but it can also be helpful to move along the leads (parallel to the package). 
	* The bridge should now be cleared. We leveraged the fact that, once molten, there wasn't enough room on the lead/pad for surface tension to "hold" the solder.
<br>

## What is soldering
Soldering is (generically) considered the act of joining things together using molten metal.
* In our context, soldering is the act of making an electrical connection- it is **not** a mechanical connection, and should not be load-bearing.
* Soldering does **not** have to look pretty. Just like anything, you'll find people that take lots of pride in their craft. However, if your goal is to quickly make a good electrical connection and appearance does not matter, then your 15 minute soldering job can be just as effective (assuming you know what to look for!) as someone who spent 2 hours making the fillets look perfect and the joints as shinny as possible. 
<br>

## What is solder
<img width="700" src="https://github.com/maholli/lab64/blob/master/soldering/images/pic1.PNG"><br>image courtesy of [nasa technical standard: soldered electrical connections](https://nepp.nasa.gov/docuploads/06AA01BA-FC7E-4094-AE829CE371A7B05D/NASA-STD-8739.3.pdf)<br>
* Solder is a combination of different metals (AKA an "alloy") that melts at a low temperature, is a strong electrical conductor, and interacts well with the metals found on circuit boards.
* The standard solder for many years was an alloy of 63% Tin and 37% Lead. Commonly known as SnPb, Sn63Pb37, or just "leaded solder."
	* Sn63Pb37 melts at about 183C
* As the industry learned more about environmental safety and hazards of lead, "RoHS" was implemented. A common lead-free solder contains Tin, Silver, Copper, and is known as "SAC305"
	* SAC305 melts at about 220C

> Special thanks to [Androkavo](https://www.youtube.com/watch?v=tfIwHuGzUEk) for his high-quality soldering footage used in this write-up.
