<h1>Energy Deposition and DPA Scoring in FLUKA</h1>

<b>NOTE:</b> To use the attached .flair file, one must have official [FLUKA](https://fluka.cern/) and [FLAIR](https://flair.cern/) installed. The .inp file can be used without FLAIR by running FLUKA through the terminal. However, it is recommended to use the flair GUI for convenience and error prevention. 

<h2>Description</h2>
The attached files enable simulation of the Mu2e proton beam on a cylindrical target. The target material is set to Tungsten, but it can be changed to Inconel-718 (defined in .inp), Graphite (default in FLUKA), or any other material in the FLUKA material library. The target has a radius of 0.314 cm and a length of 16 cm. The beam travels along the cylindrical axis, as can be verified in FLAIR's graphical geometry editor: <br/>
<img src="https://i.imgur.com/uLQVz8r.png" height="50%" width="50%" alt="Mu2e Target Model"/>
The meshing is chosen to give a satisfactory error (below 5%) for the given number of primaries per cycle (200,000 with 5 cycles total): <br/>
<img src="https://i.imgur.com/AaAKaPr.png" height="50%" width="50%" alt="Mu2e Target Model"/>

<h2>Included Scorings</h2>

- <b>Total Energy Deposition</b> 
- <b>Energy Deposition by Particle Species</b>
  - All Protons
  - Beam Protons
  - Electrons
  - Photons
  - Light Ions (Deuteron, Triton, Helium-3, Helium-4)
  - Heavy Ions (A>6)
- <b>Displacement per Atom (DPA)</b>
  - Norgett-Robinson-Torrens (NRT)
  - Athermal Recombination Corrected (ARC)

<h2>Post-Processing</h2>
For post-processing tools, see the FLUKA Post-Processing repository. 
<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
