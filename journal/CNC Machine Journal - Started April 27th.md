
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

This day probably actually took like 4 days but I'm just simplifying the days down to each like section. I know it doesn't look like much was done, but it's very complicating just jumping into it. **Total time: 8 hours**.

## Day 2 - Defining my CNC machine

On the second day I needed to define what I was actually going to build, I had already created my main constraints but now I needed to think about actual parts.

From a bit of searching around, I found that Nema 23 or higher were needed for a much bigger, rigid machine that could mill aluminum. I found a steal of a deal on **facebook marketplace**: 3, Nema 23's for just $50!! I quickly copped these steppers because I knew these were what I had to use for budget and rigidity purposes.

The next part of this day was figuring out how to build a strong frame but for cheap. I quickly realized that I didn't have many tools to cut steel or anything, so it was important that it was easily assemblable. This led me to **Aluminum Extrusions** which were cheap, rigid, and could be used to easily assembly the frame and add rails and whatnot. 

I was still very confused about what type of extrusions, 30mm, 40mm, 80mm, I had absolutely no clue and no idea what style to make them.

Something I did decide on though was a **fixed gantry style CNC mill**. I made this decision for quite a few reasons:
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

The first thing I wanted to get down was some of the base frame calculations. I needed enough space for the fixed gantry for the spindle to be able to get every part of the 40cm plate. This means that I would need 20cm of space on each side of the plate, so I decided I could probably leave the ball screw at 40cm leave (which I feel like I'll regret late) and make the rails longer for support. If the ball screw attaches to the plate at the center, this should give it a full 20cm in each direction.

I also knew that the spindle couldn't reach the farthest side of the plate because it's a big chonkier so I needed to have a little bit of space on the sides. I decided that about 5 - 10cm would suffice.

![[Pasted image 20250503190010.png]]

With this in mind, I started to design the base of the frame. I decided that 500mm extrusions for the sides and 400mm extrusions for the supports would work nicely and give me enough space.

But while putting together the extrusions, I noticed that putting the center extrusions flush with the side of the plates reduced the rigidity because there was less space in the center which was where a lot of the weight was, so I decided that fixed the inner extrusions more towards the center would increase rigidity.

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

## Day 6 - Rails and T-Nuts

I know I wanted to use T-Nuts/Bolts to bolt together the extrusions but I wasn't quite sure exactly what T-Nut to use. I'm not an engineer, so I assumed all T-Nuts were the same... But I never realized the insane variety I could get.

T-Nuts come in tons of different forms:
- Drop in spring balls - Drops in after assembly and have a ball bearing
- Double or triple T-Nut plates - multiple threaded holes
- Threaded Rod T-Nuts - have an actual like long thread that can tighten internally
- T-Nuts with stud - which come with a threaded stud
- Slide in/Preload T-nuts - insert before closing off

Here, you can be apart of the pain it is to find out what nut I need to use for this project:

![[Pasted image 20250506073552.png]]

I'm not an engineer so I had NO CLUE what to use, but T-Slot is the move!

I decided on using the slide in T-Nuts because I can attach them to the bolts and then just thread them through the extrusion and they're the cheapest ones while being extremely rigid.

But I actually might re-consider this decision because of how many T-Nuts I actually need. Tom Stanton has been a big help to visually see how to make a CNC mill, and I noticed he just uses threads to hold the extrusions together. This approach might actually be cheapest because you can just buy a threaded bolt and it would probably be cheaper. I definitely need to research this even more!

Because I started to go insane, looking at the pro's and con's of T-Nuts, bolts, etc. I decided to start looking at linear rails. Boy did I underestimate the pain this would be. Again, this CNC mill needs to be around the $300 range, but I did not think that a long piece of metal, with a rail attached would cost me $50!!!! for ONE. I needed 2 for each axis, so 6 of these.

This was a huge problem and I need to get my prices down. But thank god aliexpress is alive, I could easily get 500mm long rails for $25. But I still didn't know what type of linear rails i needed.

I thought there was only 1 type of linear rail, but nope, there's 3 major ones for CNC:
- Mainstream linear rails - just a block of metal with a rail with bearings
- Rods - a circular rod with bearings or bushings to move it along the rod
- V-Slot wheels and rails - literal wheels to travel the extrusion allowing motion

I knew that V-Slot wheels were probably out of the equation because they weren't rigid enough and it would be weird to fit them onto my extrusion that had 2 rails on each side.

So the decision was between rods and linear rails. While I feel like rods could work, I have seen next to no CNC Mill use them, and for a good reason:
- Looser fit
- Wear down pretty fast
- a bit bulkier/larger
- Noisy and flex quite a bit
- Low point of contact

So I'm probably going to use linear rails because on aliexpress, I've seen them for decent prices and I think I can get it down to maybe like $100 for all the linear rails. Costs are adding up FAST! With the stepper motors I've bought, that means I'm already at $150, but I would nearly have the frame completed, I would just need ballscrews really which I estimate are going to be like $75 or so.

But I still don't know what type of linear rails to use, the market is so flooded with chinese products, it's impossible to know what to use. A bit of a ChatGPT session later, I found out that the cheapest and most reliable rails are going to probably be MGN12's or higher (the 12 refers to the width of the rail). The thing is, the MGN's have lots of copycats on aliexpress that use the same specs, so I can get decently reliable rails for a good price on aliexpress!

The thing about ordering rails on aliexpress, is they come with anti-rust grease most of the time, so something I learned is soaking the rails in isopropyl-alchohol to remove the grease and then lubricating them so they work smoothly. This will ensure they have a long lifespan and are much more reliable, because lots of people think that the grease is actually lubricant.

Now that I kind of know what parts I want, I really want to research like the exact rail I need, because there's plenty of different lengths, widths, etc. Once I have this down, I really need to put the rails into my CAD drawing (I can probably find a good MGN rail model on grabcad) and add the T-Nuts in too.

I really want to make sure my CAD drawing is extremely precise, so I make little to no mistakes when building the actual thing irl and costing myself more money.

**Total time: 25 hours**

## Day 7 - Rethinking rails and rigidity

After putting down my thoughts on day 6, I realized that maybe my frame wouldn't be rigid enough. This was kind of a fear of mine that I didn't want to face, because this would mean rising costs and rethinking some stuff. I really want to mill aluminum on a decent scale so I need a LOT of rigidity and I'm not sure if 4040's can provide that. I'll put this on the back burner a bit and do some rails and ball-screw stuff.

While looking into where to buy my MGN15 rails, I came across lots of resource that said that MGN rails will NOT CUT IT. I did a bit more deep diving, and turns out they're really only good for light CNC like plastic and 3D printing, so I definitely needed to change this out.

Taking a bit of inspiration from the [PrintNC](https://wiki.printnc.info/en/home) I think I'm going to use HGR15's instead. These provide WAY more rigidity and will definitely be strong enough and are even rated for steel. Not only that, but these will actually strengthen the frame even further which relieves some of my thoughts about rigidity. It's also pretty much the same price as MGN15's for some reason...

There are 4 different types of HG rails though, if you want to read about them, check out [circuitist](https://www.circuitist.com/hiwin-linear-rails-guide/):
- **HGR** is the rail only
- **HGW** are carriages with **flanges** and wider hole spacing.
- **HGH** are carriages **without flanges**, taller than HGW.
- **HGL** are carriages **without flanges**, as tall as HGW.

![[Pasted image 20250506211017.png]]

*HGW vs HGH carriage*

There's tons of weird naming conventions, but I found that [Limo Bearings](https://limobearing.com/hgh20ca15ca25ca-precision-linear-bearing-rails-hiwin-equivalent?gad_source=1&gad_campaignid=21634925508&gbraid=0AAAAAoZbfAFPkPFvn4iX_BOQjB04z2VkI&gclid=Cj0KCQjw5ubABhDIARIsAHMighat6ItmEETTEZeWj1i1iQFe-XVcYvrtLyigNwKarl9bzWvAvkLdMdoaAuNmEALw_wcB) has some pretty good prices for them (but this is definitely still subject to change)!

Tomorrow, I'm pretty sure I can choose which rails I want to use and finally put them into my CAD design.

Now let's go back to talking about rigidity. I was browsing around in the [PrintNC discord](https://discord.com/invite/printnc-diy-cnc-hobby-machining-making-648972213734604807) and I kept on seeing that people suggested using steel to mill aluminum, because it's nearly 4x AS RIGID in many cases!! While I definitely still want to use extrusion for ease of assembly, I'm definitely going to consider maybe some steel parts like panels on the side.

I also really want to consider using a mix of larger and smaller extrusions in weaker and stronger spots. This is a really cool DIY CNC mill design I found in the PrintNC discord (I forgot who it was from though).

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeUsATReBbQGrH6pCXiCaGNrX0VAgS8kHitkhg_dPPRu91cT3YxJlC8oo8_LxWufcySvzPs2zTax6susLEMOqd6_l7V2FfYFMNtrVNu5DafU6yQGuZGBWSUwwCQ704yVBqqirh_HA?key=fT4XSf48xS1RgFciDTHXKleY)

The things I really like about this are they use larger extrusion on the sides and smaller extrusions for the rails which is very cool. They also use a steel frame around the whole thing, which I could imagine is EXTREMELY strong and combined with the steel side-panels, it could probably mill steel. But honestly, I could always consider building a CNC mill with only extrusion and then consider upgrading it with steel parts once it's finished.

Based off my current specs, it's definitely convincing to switch to a 30x30cm baseplate but I'm determined to make 40x40cm work. I really want to be able to mill things like keyboards at a max and 40x40 just seems perfect. I'm honestly probably going to use this idea of 2 larger extrusions on the side and 2 smaller ones inside with rails on them. 

Tomorrow I feel like I'm going to get the rails in my CAD design, look into steel parts (and how easy they are to work with) and maybe re-do/think about the frame.

There's so much to think about when it comes to a CNC mill, and I really have to consider a multitude of things and just keep on re-iterating to make something incredible and affordable.

**Total time: 27 hours**

## Day 8 - CAD, Math and rails

I really needed to get some stuff into my CAD design after doing so much research on T-Nuts and rails.

I decided to go with HGH rails because they have the highest price to rigidity ratio which is exactly what I needed. They're decently tall, very rigid and will definitely be good for this project. It's really easy to mount rails like these into the extrusion because I can just directly screw them in.

I'm really bad at CAD so it took a bit too long, but I got the rails into my design. I couldn't directly fasten into the extrusion slot because it was all at an angle, so I mounted the rails to the face and then offset them to be the center of the rails on the extrusion from looking at the specs on misumi for the 4040 extrusion.

![[Pasted image 20250507205807.png]]

![[Pasted image 20250507205851.png]]
You can see that I chose to mount them to the inner rail of the extrusion, this is because I want to evenly spread out the weight along the plate to give maximum rigidity. I still feel like the rails could be even closer to the center, but instead, I might actually just increase the size of the bed to offset the inner weight.

I found the CAD design for the rails directly on Limo (which I'll probably end up using to buy the rails), and this included the rails and the carriages.

Because the CAD design included both the rail and carriage, I had to import them separately into the assembly from my document (they came as 2 separate different parts in my part studio).

![[Pasted image 20250507210159.png]]

I then added them to the assembly by using a combination of planar mates to be able to move them along the Y, a fastened mate with an offset, to put the perfect distance between them, and then I grouped all 4 rails after offsetting them so they slide together.

![[Pasted image 20250507210343.png]]

I did some really annoying math using the carriage and the dimensions of the baseplate to properly align them.

![[Pasted image 20250507210437.png]]

Next I added the bed into the CAD design. I'm heavily considering switching to a 30x30cm work area for rigidity which I know wasn't my initial goal but I feel like it's for the best. It gives nearly 2x the rigidity and will have a way higher likelihood of milling aluminum at a good rate. I might be able to sneak in a couple cm too along the X or something but I'll see.

Because I'm really considering making it smaller, I designed the baseplate off 30x30cm dimensions. I did all the annoying math and put the screw holes so there's enough clearance for them to fasten to the rails. I also put a chamfer on the top of the holes for the screw head.

![[Pasted image 20250507210757.png]]

Then I simply mounted it using another hole for reference using a fastened mate and now we have a fixed gantry.

![[Pasted image 20250507210841.png]]

**While this all looks pretty good, there's LOTS OF PROBLEMS, here's a couple:**
- Enough clearance for the screws and the proper space for a clean chamfer.
- The rails probably need to be longer so the mil can touch the middle of the base-plate along the Y axis
- Slight misalign of the screw holes for some weird reason (shown below)
- Proper bed thickness and dimensions for maximum rigidity and screw depth
- Proper frame dimensions to accompany the new bed size of 30x30cm

![[Pasted image 20250507211033.png]]

(weirdly aligned screws)

So tomorrow, I'll probably work on fixing all these issues, because I CANNOT have too many issues when I'm assembling the whole thing. Costs add up FAST. I also maybe want to do some sponsorship outreach (which might be better for the weekends). But aside from that, my CNC mill design is really coming together, it's definitely hard work, especially because of the fact that I'm not an engineer and in school for 6 hours a day :(.

**Total time: 30 hours**

## Day 9 - Adjustments and research

I added a lot of stuff to the CAD design yesterday, but a lot of it was added in a sloppy way, so I really needed to clean up my design.

The main problems/errors I had were:
- Screw clearance (which I thought was probably good, I'm probably going to come back to this later)
- Too short of rails (which was definitely a problem)
- Misaligned screw holes (another massive problem)
- Proper bed thickness (definitely still an issue)
- Frame dimensions for the new 30x30 bed (definitely an issue too)

I felt like I could comfortably ignore the screw clearance because I know I'll probably come back to it when researching all the proper screws, bolts, t-nuts I need and whatnot so I didn't want to worry about that right now. I definitely needed to get these other issues fixed though.

First I focused on the rails being too short. I had 2 options of fixing this:
- Increase the length of the rails, affecting rigidity, possibly having to make the machine larger
- Decrease the distance between the 2 carriages on each side, maybe affecting rigidity

I decided to go with the latter because the rails were only about 1cm too small in total (on both sides). This means, I'd only have to decrease the distance between the 2 rails, by 1cm which doesn't have a massive impact. I'll definitely be running simulations later to test how strong this will actually be though.

Because the center of gravity was a bit wack on the bed now, I decided to increase the side of the actual plate to offset some of the stress put on the center of the bed. So now the bed is 35x35cm which means the bed will be approximately 5kg, which will give the machine some more heft and rigidity.

Fixing the screw holes was pretty easy (but a bit annoying). I re-calculated the whole positions (with the new carriage placements too) and it seems work well. There still seems to be a tiny offset though which is a bit bizarre, I think it might be because of mistakes with the model, but I might revisit it, if I deem it a problem later on.

![[Pasted image 20250508203738.png]]

*Straight on view of the weird holes*

Because I was making the work area a full 10cm smaller, I could comfortably decrease the width of the frame from 580mm to 480mm, which will give a big boost to rigidity and make my mill much more capable of milling aluminum and giving it long-term strength. I honestly think this decision is for the better, and will probably save me time, money and pain.

Now the mill was looking much better and much stronger, I increased rigidity, fixed many small errors and made some good progress. I'm still really horrible at designing as this is my first major engineering project I've worked on.

But now, I needed to work on some pressing matters. The X and Z axis. I always wanted to do a fixed gantry style machine, because I knew that supporting the whole gantry on rails and ballscrews would need to be horribly rigid and cost lots of money in the process.

With a fixed gantry style, I could just mount sideplates and then attach the gantry, being very rigid. The thing is though, you can't create the side plate out of anything. Extrusion probably wouldn't cut it, being the gantry is a lot of weight, and the extrusions will probably bend underneath the sheer pressure of a mill.

So I have a few options for the side panels:
- Multiple, rigidly mounted extrusions on the side
- Solid aluminum plate with drilled holes (pretty thich)
- Solid steel plate with drilled holes (maybe welded?) (less thick than aluminum)

I'm still debating what to do, and I need to look more at the pro's and con's of each, but I feel like extrusion might not be an option. I feel like it just doesn't have the rigidity to support the most important part of the CNC mill, and it'll probably be quite pricey to make it work.

> "A Chain Is Only as Strong as Its Weakest Link"

The problem with working with aluminum and steel though is I'll probably need to drill custom holes, and have a custom sheet cut to what I need it to be probably like so:

![[Pasted image 20250508205736.png]]

But this gives an insane level of rigidity, and I could definitely mount another slab on-top for the X axis. Tomorrow I'll look into more options for this, and I also want to take a look at BALL-SCREWS!!! I didn't get too much time to work on but I still got a solid amount done!

**Total time: 32 hours**

## Day 10 - Reinforcements and side plates

I've decided that it's definitely better to go with a 4080 frame vs a 4040 frame. I want to modify my layout so it uses 4080's on the outside, and then some 4040's in middle to support the rails.

I feel like this is honestly a necessity, because to be able to mount the side-plates, I need to have a strong enough mount which only the 4080 provides. I also definitely need some more rigidity to be able to be able to mill aluminum.

The 4040's I'm probably going to use for the center, will also be a different style from the ones I used before. Instead of having 2 rails, they'll just have 1, they look like this:

![[Pasted image 20250510205535.png]]

**Instead of** 

![[Pasted image 20250510205544.png]]

These 4040's are a tad bit more expensive, but they're way more compatible with the 4080's than the 2 rail ones and are a bit more rigid.

Now I have to actually rebuild the frame in my design.

First off I got the basics of the frame down. The outside is 4080's and the 2 inner beams are 4040 (which I'll maybe turn into 4080's).

![[Pasted image 20250510224517.png]]

~~The beams are going to be attached by 4 T-Nuts on each beam and maybe some other supports on it too.~~

After a bit more research, using T-Nuts probably isn't feasible. Maybe using T-Nuts with something else could work, but probably not. I've been looking at a couple other options though:
- Internal corner connectors (rigid and cheap, basic tools)
- Diagonal bracing on some areas to make it stronger, like the side panels
- Plate that attaches the corners
- External connectors of some sorts
- Maybe some T-Nut stuff, I'm not too sure

I'll have to look into this a bit more, but for now I wanted to fix my CAD drawing so that it included the 4080's and 4040's instead of the old 4040's with 2 rails.

It wasn't too complicated to change (though it probably took me too long because I kinda spent too long fixing really minor mistakes I was making), but I finally got it done, and it was looking RIGID. I feel like this is the perfect price/rigidity ratio, and I Feel like it will work perfectly, especially with the strong linear rails!

![[Pasted image 20250511211941.png]]

I'm planning on probably doing aluminum plate, maybe like 10 - 12mm thick, for the side panels, because they need to be one of the most rigid parts of the machine and I feel like plate is probably the cheapest way to get that.

I feel like my budget might be going a bit over, but luckily Hackclub is about to release their next event where I'll be able to get a $350 grant for my project, which will hopefully allow me to build this for little out of pocket! (I might even get to go to San Francisco too!). I'm estimating the project will probably come out to a bit over $400, more than the $300, but I like to set really hard goals and then fall short a bit, but still over-perform!

So for tomorrow, I really need to think about how I'm going to actually connect these extrusions and what I'm going to do for side panels. I haven't had much time in the past 3 days to work on this, so I'm glad I'm finally getting an update out. This update probably took me about 3 days, but I still got quite a bit done, and I can definitely feel like skills improving. I also still want to maybe reach out to some local companies about sponsoring, especially for the side panels, which would be a LIFESAVER!!

The CNC mill is coming along amazingly well, and it's really motivational to see a realistic frame come out, and I'm really excited to keep on working on this.

**Total time: 36 hours**

## Day 1 - Fastening

I found this really cool build guide that shows all the steps in building an [Avid CNC](https://www.avidcnc.com/support/instructions/rotary/assembly/) . It gives me a lot of cool ideas on fastening.

Personally I feel like I'm going to go with a mix of T-Nuts, internal connects and external brackets and now I'm also looking at anchor fasteners.

![[Pasted image 20250512065201.png]]

*Anchor fasteners* 

I found [this tutorial](https://toolguyd.com/hardware-for-connecting-t-slot-aluminum-anchors-end-fasteners-brackets/) gives cool ways of attaching 4040 together. It's honestly pretty boring researching different ways of fastening stuff together, but now that I had a bit of an idea how to fasten stuff I wanted to do some side panel stuff and maybe work on the X axis a bit.

There weren't many resources on side panel dimensions so I kind of winged it, but I knew it had to be rigid, and that the Z height couldn't be too large or it would decrease rigidity and maybe move a bit. So I did a bit of calculations and decided I wanted a clearance of at least 10cm, so I kind of just arbitrarily set the Z height to be 250mm. This gave me 13cm of clearance and I think it's going to work. I feel like it's probably not hard to make it taller or shorter if I need, but this gives me a good amount of space while keeping rigidity in mind. I also just made the side panels 12mm thick, and 15mm wide, I'm honestly not too sure how big to make them, but it's easily changeable.

![[Pasted image 20250512184520.png]]

Next I wanted to work on something a bit new, the X axis. The X axis is going to be between the 2 side panels and needs to be long enough to clear the work area while maintaining rigidity. There's tons of different ways of attaching the X axis on:
- Bolting extrusions to the side panels, and then mounting rails onto those
- Bolting a beam or another extrusion to the top face of the side panels and then attaching the rails onto that.
- Bolting an extrusion or another panel to the front or back face of the side panels
- And there's probably a couple other ways but those are the main ones

I also recently found this site called [open builds](https://builds.openbuilds.com/?category=cnc-router-builds&id=286) that literally just has like hundreds of hobby cnc mills, routers, lathes and so much more. This is going to be a massive spot for inspiration on design ideas and whatnot. Personally I feel like I probably want to just bolt some extrusion to the side panels and then mount the rails onto them. 

I can either bolt 2 smaller 4040's or something to them, or one big extrusion panel to act as a face, and I feel like the price difference isn't actually huge so I'll just compare rigidity. I feel like maybe using some extrusions to support the beams in the dead-space beside the bed too would make it even more rigid.

Overall it was a really boring day of just researching and brainstorming. I know it probably looks like I didn't do much, but I'm spending a lot of time on the brainstorming so I can maximize the success of my project. I feel like people don't use enough thinking on their projects these days, but it's really what the key to a perfect product is.

It was also next to impossible to find resources on connecting 4080 for CNC mills, so I had to really dig to find information, they'res no good tutorial or overview on how to make a CNC mill so that's really what I'm trying to do. So now I have a really good idea on how to connect the extrusions, I also pretty much know how I'm going to do the side panels and also the beam between the side panels.

Tomorrow I really want to get the beams into the CAD design (along with the rails) or work on connections which I always like procrastinating.

*If you got this far into the log so far, just remember:*

> **Perfection in Details** - Steve Jobs

**Total time: 39 hours**