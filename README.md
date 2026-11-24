# EX-No.6.1. DESIGN THE VARIOUS PARTS OF A MECHANICAL COMPONENT AND ASSEMBLE

## DATE: 19.11.2026

## AIM: 
To Design the various parts of a mechanical component and assemble it using a bottom-up approach then convert it into the orthographic view

## REQUIREMENTS: 
1. Autodesk fusion 360
2. Windows 10
3. 4 GB of RAM (integrated graphics recommend 6 GB or more)
4. 2.5 Mbps or faster download; 500 Kbps or faster upload 


Select the objects to modify then specify the distance or angle. Use set pivot to reposition the manipulator

## PROCEDURE:

## Phase 1: Part Modeling
(Set default document units to Millimeters (mm) and hybrid mode to make components before starting).
## STEP 1: Base Plate (BASE PLATE)
Start a sketch on the XY plane and construct the outer polygon profile using the given dimensions (20 mm, 26.47 mm, 30 mm, 20.62 mm, 25 mm, 27.8 mm, 14.2 mm, and 20 mm).
Create the internal 15 mm slot with R3 rounded ends.Add the mounting holes: Ø6 mm holes at the upper and left positions, and Ø4 mm holes at the bottom mounting points.Extrude the base profile to a thickness of 4 mm.

<img width="556" height="436" alt="Screenshot 2026-11-24 115626" src="https://github.com/user-attachments/assets/923ae279-9974-4673-b183-42228bc77c58" />
<img width="625" height="367" alt="Screenshot 2026-11-24 115636" src="https://github.com/user-attachments/assets/71b77172-9f66-4508-ba66-37e6796f3348" />

## STEP 2:Linkage (LINK)
Create a new sketch on the XY plane.
Draw two circles of diameter Ø6 mm spaced 45 mm apart (center-to-center).
Draw two outer concentric circles of diameter Ø10 mm (R5) around the Ø6 holes.
Connect the two circular ends with a rectangular web of width 5 mm and apply tangential fillets/trims to match the 36.34 mm inner span.
Extrude the closed profile symmetrically or in one direction by 4 mm.Assign material as Steel and save the component.

<img width="445" height="503" alt="Screenshot 2026-11-24 115734" src="https://github.com/user-attachments/assets/a4b595b7-8530-4630-9ccb-bcee804cb6d9" />
<img width="430" height="333" alt="Screenshot 2026-11-24 115739" src="https://github.com/user-attachments/assets/3542307a-415f-4c8e-83d1-dc68a420169f" />

## STEP 3:Gear Linkage (GEAR LINKAGE)
Create a sketch on the XY plane and draw the main gear head circle of radius R15 mm with a central bore of R3 mm (Ø6 mm).
At the bottom of the arm, draw the pivot hole of R3 mm (Ø6 mm) and outer arc of R5 mm, connected by a 6 mm wide arm (overall length 71.97 mm).
Sketch a single gear tooth profile using Detail A (1 mm tooth thickness, 0.47 mm addendum, 2.06 mm pitch spacing) and use the Circular Pattern tool to replicate the teeth along the sector.Extrude the entire profile by 4 mm and assign Steel as the material.

<img width="552" height="596" alt="Screenshot 2026-11-24 115904" src="https://github.com/user-attachments/assets/67e3a6e7-5290-4300-9f3c-47d031d2eb58" />
<img width="340" height="375" alt="Screenshot 2026-11-24 115910" src="https://github.com/user-attachments/assets/1ee2cde8-ddf5-4b7d-9d7f-bc34f1f8e703" />
<img width="427" height="272" alt="Screenshot 2026-11-24 115915" src="https://github.com/user-attachments/assets/de4f4fc5-0cca-400b-9177-b8252ded37bd" />

## STEP 4:Finger (FINGER)
Create a sketch on the XY plane and draw the lower pivot section with two R3 mm (Ø6 mm) holes spaced 25 mm apart, bounded by R6 mm outer arcs.
Extend the angled finger body at 154.44° with a total length of 113 mm (overall height 149.84 mm), incorporating the 30 mm step, R3 fillet, 74 mm upper grip edge, and 44.96° chamfered tip.Extrude the sketch to a thickness of 10 mm, assign Steel, and save.

<img width="376" height="517" alt="Screenshot 2026-11-24 120039" src="https://github.com/user-attachments/assets/4d3f4be6-05ee-4f52-89dc-38512a9a93d4" />
<img width="381" height="481" alt="Screenshot 2026-11-24 120044" src="https://github.com/user-attachments/assets/e749144e-f8ab-41a0-afee-e71dcd02c7c5" />

## Phase 2: Assembly & Motion
Create a new design file and save it as Robotic_Gripper_Assembly.
Insert the BASE PLATE into the workspace, right-click it in the browser, and select Ground to fix it in space.
Insert the required quantities of the remaining parts:
 1.GEAR LINKAGE (Qty: 2)
 2.LINK. (Qty: 4 — two upper, two lower)
 3.FINGER (Qty: 2)
 4.Standard pins/fasteners (if modeled) to secure the joints.
Apply Revolute Joints (J shortcut) to connect:
Both GEAR LINKAGE central holes to the corresponding pivot holes on the BASE PLATE.
The LINK. ends to the BASE PLATE and FINGER pivot holes to form the four-bar parallel linkage mechanism.
The lower pivot holes of the GEAR LINKAGE arms to the FINGER pivot points.
Enable Contact Sets (or apply a Motion Link between the two gear linkages with a -1 ratio) so that rotating one gear drives the second gear and opens/closes both fingers symmetrically in parallel.

<img width="512" height="548" alt="Screenshot 2026-11-24 120515" src="https://github.com/user-attachments/assets/4997d4ea-9cf8-460f-9122-257c7c879f1f" />
<img width="743" height="441" alt="Screenshot 2026-11-24 120520" src="https://github.com/user-attachments/assets/cf58db4e-283f-4f07-82c3-df25728b7767" />
<img width="725" height="597" alt="Screenshot 2026-11-24 120526" src="https://github.com/user-attachments/assets/6871e509-db42-41f2-8a75-8b939a42cf5b" />
<img width="707" height="617" alt="Screenshot 2026-11-24 120537" src="https://github.com/user-attachments/assets/b8710c2a-f475-46e5-800b-298442ce9135" />

## COPY ALL COMPONENTS AND ASSEMBLE ON THE OTHER SIDE:

<img width="680" height="452" alt="Screenshot 2026-11-24 120542" src="https://github.com/user-attachments/assets/d6ad7469-57a3-4a9a-88d0-1ade7a678811" />
<img width="696" height="582" alt="Screenshot 2026-11-24 120547" src="https://github.com/user-attachments/assets/6d09eca9-1ac7-4539-bcd7-c79de9421c46" />

## INPUT: 

#### LINKAGE
![image](https://user-images.githubusercontent.com/113594316/199413513-8fa5b9db-0546-49d0-ad4c-230b22984d3c.png)

#### BASE PLATE  
![image](https://user-images.githubusercontent.com/113594316/199413545-3b2fd515-6e27-4d28-9da3-c9ce20cb2a42.png)

#### GEAR LINKAGE
![image](https://user-images.githubusercontent.com/113594316/199413566-05708531-fc78-44c9-ab98-4f8a9066d318.png)

#### FINGER
![image](https://user-images.githubusercontent.com/113594316/199413594-5de9578e-5800-4e69-8c76-6a5749e31805.png)

#### ASSEMBLED VIEW
![image](https://user-images.githubusercontent.com/113594316/199413636-df0a61ce-964f-490d-9a16-e5986ebbf403.png)

## OUTPUT:
<img width="837" height="538" alt="Screenshot 2026-11-23 234326" src="https://github.com/user-attachments/assets/c681fd40-cd46-4421-9813-329d67be94df" />
<img width="926" height="655" alt="Screenshot 2026-11-23 234228" src="https://github.com/user-attachments/assets/b60289c4-b55d-4b75-9066-7ff31d4c327e" />

## RESULT:
Thus, a design of various parts of a mechanical component and assemble it using a bottom-up approach in orthographic view has been done

ILANILA VINNARASI.K.V
26017175
19.11.2026


