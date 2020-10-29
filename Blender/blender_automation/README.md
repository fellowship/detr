# Blender Automation

Blender Automation is a high level command line interface to develop a scene(s) in blender and render it to a image file(s).
This module aims to remove the knowledge gap between Blender Experts and Python developers, though this module does only the basic works.
It's targeted towards the generation of the Synthetic Image dataset generation with the automatically generated annotations for object detection.

There are sub-modules as follows:
* __Blender API__ :
	* __BlenderObject__ : BlenderObject Class provides methods to change the geomentrical details along with the placement and provide functionality like Importing an object and deleting it
	* __BlenderScene__ : This class manages the Scene in blender, keep track of objects in it
	* __BlenderCamera__ : Provide method to change the geographical parameters for the camera to get different images from the created scene
* RenderInterface : This module is the command line interface to create a scene and manage it, with the functionalities like automatic placement(To be implemented) and importing object in to the scene or deleting it, (might be more to it, not now)


script src/__render\_poses.py__ is the script that is to be passed in blender for the whole process

script __rendering\_pipeline.pt__ : [NOT DEVELOPED] arranges all the arguments containing the paths for the necessary files (haven't decided it yet... might not use it at all)

### How to use:
Lookup in Documentation here[WIP]

To begin with for now you can run: `blender --python render_poses.py`, there is a class method `dry_run()` for testing purpose, which has manually generated blender scene