# OpenFOAM-ESB-testcase
Step 1: First install openfoam. Complete all steps till you have successfully completed Openfoam cavity tutorial
Step 2: Download this folder and Unzip it. Move it to your openfoam/<user-name>/run folder
Step 3: Type "blockMesh" in the command line without the quotes and press enter. (empty domain mesh with blocks)
Step 4: Type "topoSet" in the command line without the quotes and press enter. (create the cube structure inside the domain)
Step 5: Type "snappyHexMesh -overwrite" in the command line without the quotes and press enter. (create the cylinders on top of the cube)
Step 6: Type "checkMesh" in the command line without the quotes and press enter. (to see if the final mesh is ok)
Step 7: Type "simpleFoam" in the command line without the quotes and press enter. (run the solver)
Step 8: Type "paraFoam" in the command line without the quotes and press enter. (Follow parafoam tutorials to explore more)
  
To view the domain and structure,
  1. Look at the left part of your window. in the properties tab,scroll down till you find Mesh parts.
  2. Select all.
  3. In the third row, there are 3 dropdowns. One of them will have the option "Wireframe". Select that.
  
To see the velocity field on the structure,
  1. Look at the left part of your window. in the properties tab,scroll down till you find Mesh parts.
  2. If step 3, 4 and 5 are performed correctly, you should see porousCells and support. Only select these two, deselect the rest.
  3. Click apply. You might have to rotate the layout to see. Click and move the cursor on the image to rotate and align.
  4. On the top, in the third row, you will see a drop down menu with "vtkBlockColors" selected. Drop down and pick U, the one with a circle in front of it, not the diamond.
  5. Check that the drop down next to it is "Magnitude", and the one after is "Surface".
  6. On the right hand side, there is a Color Map Editor (View -> Color Map Editor, if it is not visible). 
      Near mapping data, there is an envelope with a heart on it. that is to choose your color range. I pick rainbow uniform.
  7. To rescale the data to all the time steps, In the third row, select the 6th button. It looks like a timeline with a t on top it.
  8. In the second row, there is a play button -- to go through all time steps. you can push the button on either side to see the next or previous frame.
