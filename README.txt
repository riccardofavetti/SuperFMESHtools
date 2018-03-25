#######################################################

SUPER FMESH TOOLS V 1.0

Coded by R. Favetti with Python 3.6 and Kivy 1.10
contact: https://www.linkedin.com/in/riccardofavetti/

#######################################################

1. What is Super FMESH tools?

	Super FMESH tools is a utility to handle MESHTAL files
	produced by MCNP as a result of FMESH tally analyses.
	There are 3 functions implemented:
	1. File loading:
		once files are imported, an output file is produced
		in the working directory. The output shows information
		about the imported files.
	2. Sum meshes:
		results of two meshes can be summed voxel by voxel
		provided that the two meshes are the same.
	3. VTK writing:
		a 3D representation of mesh results can be achieved
		writing a vtk file. The vtk file can be handled using
		the software "Paraview".
		The result of a sum can be exported into a vtk file as well.


2. I have a meshtal file, how can I import it?

	To import a meshtal file you need to do the following:
	1. Add the extension .mesh to your meshtal file
		e.g. "meshtal" becomes "meshtal.mesh"
			 "genericname" becomes "genericname.mesh".
	2. Choose the directory where the file is in Super FMESH tools.
	3. Click on "Load meshtal files"
	
3. Can I import more than a meshtal file at once?
	
	Yes! Just mind to add the .mesh extension to all the files 
	to be imported before clicking on "Load meshtal files".
	

4. Which information is shown in the output file SuperFMESHtools_out.txt?
	
	The following information is available:
	
	- number of voxels
	- max tally value
	- max error value
	- number of voxels with relative error values less than or equal to 0.05
	- number of voxels with relative error values less than or equal to 0.10
	- number of voxels with relative error values greater than 0.10
	