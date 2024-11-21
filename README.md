# So many options, so little time

As I started designing a simple 3D fin can that a group of young students could use to assemble and fly a model rocket quickly, the idea of scaling up the design quicky followed. 

13mm to 18mm to 24mm motors. BT-20 to BT-50 and beyond. Combinations and Permutations. Where does it end? 

I framed the design space with a matrix that mapped out the possibilities and assigned them 'working names' associated with the motor size in millimeters and body tube per the Estes designation. 

For example, the Ez3D-1855 supports an 18mm motor with a fin can that transitions to a BT-55 airframe. 

But how long of an airframe? My original design used a 6-inch portion since I could cut the commercial 18-inch length into three 6-inch segments. Models with larger motors required a longer airframe so a 9-inch (i.e. cut the 18 inch tube in half) and 18-inch lengths came naturally. 
The dashed number at the end of the Ez number indicates the length. 

I decided all models would have four fins of 2mm thick. This helps with printing surface plate adhesion (although using a brim and plenty of glue stick really helps too). 

I then choose which models from the matrix would graduate from an 'engineering designation' to a 'marketing name'. They follow a natural progression of increasing motor case sizes and body tube diameters but in reality, any of the mixing and matching would work just fine. If you want to modify one of the FreeCAD drawings and make your own variation - please do! That is why all the files and this methodology are here. 

The matrix design space could keep going: Q-jet, Enerjet, Micro-MAXX, CTI, DMS, RMS. But the goal was to set you up with the tools for your own success. 

Note: Most performance numbers are not verified. Initial cuts are from sim data and a few of the low power versions are updated with flight data. I'll update the sheet as more data becomes available. 


																								
![image](https://github.com/user-attachments/assets/35f45614-4c75-4829-acb3-d296985933b8)

# Motor Retention - the biggest challenge

All the designs incorporate a threaded base with a 'retaining nut'. It looks easy now but look a long time to incorporate. Here's why:

1. Although FreeCAD can make bolts, it is difficult to add external threads to an existing column. Yes, there are several work arounds on YouTube and forums but none worked out well.
   - The external threads were made with Autodesk Fusion, exported as a .stl file, and added to the existing fin can drawing in FreeCAD. Files included above.
   - When exporting the FreeCAD part into a STL file, be sure to also select the threaded base.
2. FreeCAD does have a feature to make a threaded hole. This is used to make the motor retention retaining nut.
3. Even though I selected the same thread parameters on the but and bolt, the fit was too tight to work. That's why there are scaled up versions of the retaining bolt.
    - +3% and +5%  in the X and Y direction were sufficient to get a good fit for the first flight
4. After the first flight, the scaled up retaining nuts no longer fit due to the PLA shrinking from the heat. That's why the small retaining nuts are included.
   - I chose to stick with PLA since that's what most of us 3D printing noobs use.
5. I tried several ways to incorporate metal motor hooks but the complications were not worth it.

# Motor Mount Shrinkage - the other challenge
The goal is to make a model that can be built with PLA filament since it is most common and used by beginners. However, PLA tends to shrink after heating which causes the motor mount area to shrink. 
After a few flights the motors may become stuck or unloadable. 

To mitigate this, a tapered motor mount tube is used. The motor has a loose fit but maintains centering with the top sloping of the traditional "Engine Block" and the aft section is narrower and relatively cool from insulating effect of the clay nozzle. 
 - Note: The sloping of the "Engine Block" was to make it "3D printable" without supports. The 'centering' effect is now an added benefit.

 - Currently only the Ez3D Mini has been test flown in this configuration. After three flights, the motors showed no signs of tightness (Ref: flights on a 70deg cloudy day).

# It's the little things
- The early version of the 1850 used a 6 inch tube and single launch lug on the fin can. During a C6 flight, the fin with the lug snapped off while heading up the rod (the rod was rusty rod which may have contributed). Fortunately the model went downrange but now the 1850 model includes the tube launch lug (same reasoning with the 18PT). It's also now a 9 inch tube to increase stability margins with heaver motors.
- Ejection charges from larger motors cause more melting damage to the tube adapter section that holds the recover harness. Some of the larger models have a 2mm thick wall to increase durabilty.
- A 4mm internal diameter works fine for a 1/8" launch rod but I increased it to 4.5mm to allow for rods with 'imperfections'.
  
