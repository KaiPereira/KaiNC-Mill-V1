
## Day 1 - Brainstorming

On the very first day, I set out defining the goals I wanted for this project and actually learning about the pain of making a CNC I'm going to go through.

Here's the main criteria I wanted for the machine:
- At least a 40cm x 40cm workspace, perfect to machine literally 99% of things
- Cost around 300 USD, so it's affordable for me and others
- Be able to mill aluminum, plastic, wood and mdf
- Be decently small and contained
- Easily repeatable for others
- Easily assemblable because I had very minimal tools

The 300 USD budget is very ambitious but it's something I thought was really important, because I feel like the whole point of making a CNC machine is to make it budget friendly for anyone anywhere.

I found a lot of really good resources like the [Infill](https://infill.hackclub.com/overview/getting-started) page which details how to make a 3D printer and I feel like 3D printers are directly relatable to CNC machines.

This taught me about the basics of a CNC machine:
- Having a frame
- Rails to guide the axes
- Something to move the axes like ball screws or something
- Spindle

I had a good idea of what a CNC machine was actually made with by the end of first day.

This day probably actually took like 4 days but I'm just simplifying the days down to each like section. **Total time: 8 hours**.

## Day 2 - Defining my CNC machine

On the second day I needed to define what I was actually going to build, I had already created my main constraints but now I needed to think about actual parts.

From a bit of searching around, I found that Nema 23 or higher were needed for a much bigger, rigid machine that could mill aluminum. I found a steal of a deal on **facebook marketplace**: 3, Nema 23's for just $50!! I quickly copped these steppers because I knew these were what I had to use for budget and rigidity purposes.

The next part of this day was figuring out how to build a strong frame but for cheap. I quickly realized that I didn't have many tools to cut steel or anything, so it was important that it was easily assemblable. This led me to **Aluminum Extrusions** which were cheap, rigid, and could be used to easily assembly the frame and add rails and whatnot. 

I was still very confused about what type of extrusions, 30mm, 40mm, 80mm, I had absolutely no clue and no idea what style to make them.

Something I did decide on though was a **moving gantry style CNC mill**. I made this decision for quite a few reasons:
- The Y axis can be controlled by one stepper motor and uses less material because a fixed style needs to have decently long, very rigid steppers on both sides of the machine with longer ball screws and more expensive parts used to make it work.
- It's a very rigid and efficient design that will maintain strength but also be decently cheap still

Using all this information I created my first drawing. Drawings REALLY helped define what I was building and were probably one of the most important aspects of building such a crazy machine. **This is a basic drawing I did in Krita:**

![[Pasted image 20250503114651.png]]

You can see that the frame is purely made out of aluminum extrusions and bolts which make the frame pretty cheap and easy to assembly because I can just order the extrusions to size and with the specs I want.

**Total time: 12 hours**

## Day 3 - Collecting my thoughts

The big thing I wanted to do on day 3 was to get my thoughts down and actually to start working on a CAD design.

I knew I wanted to create the frame out of aluminum extrusions but I still wasn't sure what type of aluminum extrusions to use. This is where Tom Stanton came in clutch. His series on [building a CNC mill/router](https://www.youtube.com/watch?v=t7yjEYOrYFo&list=PL04nKdxcTrP1Q1D6-LQL-cWMClAlg0pY2) was a massive help to me, because he showed the full general process of building exactly what I wanted to do.

I noticed that Tom Stanton used extrusions that had 2 slots in them like this.
![[Pasted image 20250503115326.png]]
This gives lots of space to add rails and connect segments, while maintaining a very high level of rigidity. I still didn't know where to order them from though, so a quick google search later and I come across **Misumi**. I couldn't believe that I could get 4040 extrusions that were 400mm long for just **10 USD** and I could fully customize them!!! 

At this point, I'm pretty sure these are the extrusions I'm going to go with, but I still want to keep the price cheaper so if I somehow come across something cheaper and as high quality I might go with that.

Now I still wanted to actually get something on paper, so it was time to do a bit of CAD work. I've decided to use [Onshape](https://www.onshape.com/en/) for my CAD because it works in the cloud so I can still work on this in school and I'm used to using it for other projects. I might switch to Fusion360 though if it gets too laggy, but we'll see. 

I'm not used to creating huge assemblies like this in onshape, more designing parts so I referred to ChatGPT really quickly on how to create an organized workspace. I figured out the easiest way would be to add in the DXF's of things like extrusions, then create part studio's for all the sub-assemblies like the aluminum extrusions. Each sub-assembly would have like the different sized of extrusions like 400mm long, 800mm long, ect. And I will probably end up doing this for all the different parts like linear rails, ballscrews, etc.

For the end of this day, I finally got something into my CAD workspace and it's so cool to actually get something on paper though after 10's of hours of brainstorming. 

![[Pasted image 20250503120536.png]]

Just 2 simple aluminum extrusions but it's really exciting to see something actually on paper.

**Total time: 16 hours**

## Day 4 - working on the frame and revisions

I knew this day would be a bit slow because I was starting to put some stuff on paper and making many revisions to my vision.

The first thing I wanted to get down was some of the base frame calculations. I needed enough space for the moving gantry for the spindle to be able to get every part of the 40cm plate. This means that I would need 20cm of space on each side of the plate, so I decided I could probably leave the ball screw at 40cm leave (which I feel like I'll regret late) and make the rails longer for support. If the ball screw attaches to the plate at the center, this should give it a full 20cm in each direction.

I also knew that the spindle couldn't reach the farthest side of the plate because it's a big chonkier so I needed to have a little bit of space on the sides. I decided that about 5 - 10cm would suffice.

![[Pasted image 20250503190010.png]]

With this in mind, I started to design the base of the frame. I decided that 500mm extrusions for the sides and 400mm extrusions for the supports would work nicely and give me enough space.

But while putting together the extrusions, I noticed that putting the center extrusions flush with the side of the plates reduced the rigidity because there was less space in the center which was where a lot of the weight was, so I decided that moving the inner extrusions more towards the center would increase rigidity.

![[Pasted image 20250503190111.png]]
Now I modeled everything into Onshape using these revisions and calculations, and created a basic base frame.

![[Pasted image 20250503190202.png]]

This base will be rigid yet compact and leaves enough space for spindle to hit everywhere on the plate. I still feel like I need to center the extrusions a bit more, but I'll see when I put the plate actually in the CAD design. 

I want my CAD file to feel like literal instructions for building this so I might turn away from the frame for a day or two so I can actually CAD the bolts and stuff that will connect the extrusions.

**Time total: 18 hours**

## Day 5 - Disaster and Progress

This day made me some reality checks and I also made a lot of progress. The main focus initially of this day was to get fastening of the joints down into CAD.

I had absolutely no clue how to fasten aluminum extrusions and the internet actually wasn't that helpful. So I did some deep research and decided that a bolting with T-Nuts would be the easiest option.

This process is a bit complicated to understand at first, but it's fairly simple:
- Tap both ends of the 400mm extrusions
- Screw in bolts and T-Nuts into the tapped ends
- Cutting holes that match up with the T-Nuts into the 500mm mounting extrusion
- Slide the T-Nuts into the 500mm mounting extrusion
- Tighten the bolt to create a very solid mount

So I added the holes on the mounting extrusion and this is where some things started to go downhill.

![[Pasted image 20250504203611.png]]

I've realized that I want to make the machine mill 40cm x 40cm but my extrusions are only 4cm. I thought 4cm was a decent amount but I took a quick look at a measuring tape and realized it was pretty tiny.

I also realized I completely messed up my frame calculations, just how big the mounting extrusion is going to be and how much extra space I'm going to have on the sides. So this means tomorrow I'm going to have to spend a lot of time doing re-calculations and more research.

![[Pasted image 20250504204156.png]]

I really want to be able to mill aluminum, so that means the design needs to be RIGID, but I also want to be able to mill 40cm x 40cm, so I feel like I either have to make the working area of the CNC mill to be smaller, or make the extrusions bigger.

I still want this to be very budget friendly though, and making the extrusions bigger, increases the cost quite a bit (nearly double), so I'm going to have to think of a smart way of solving this.

I could use 4080 extrusions, or maybe use like mounting brackets to make it stronger, but I'm not too sure.

Now time to make some more revisions. First off, I redid the calculations (this is probably my favorite drawing so far):
![[Pasted image 20250504205838.png]]
I now have an accurate frame with 5mm of error on each side, and keeping maximum rigidity in the center of it (which is the second revision of the drawing)

Now time to put update my CAD design! I keep on messing up my calculations because my drawings are from the edges of the extrusions instead of the middle of the holes, but after a couple tries I got it down. much more rigid now!
![[Pasted image 20250504211226.png]]

Now I still might actually put them closer together, but I'll take a look at it once the rails are actually on it. For now, I want to research if I need larger extrusions and I want to get the T-Nuts and bolts into the design.

**Total time: 22 hours**