# TouchDesigner-AE-Import
TouchDesigner 088 component that imports keyframes from After Effects layers exported into text files.

##Build and Version
This tool requires 'Custom Parameters' functionality within TouchDesigner (Build 45000 and above). It was created, and is stable, in 64-bit build 61480.

##Installation
1. Add the ```nVoid_AE_keyframe_importer.tox``` component into your project.

##Notes about After Effects
Copying Keyframes :
Keyframes can only be converted to text from one layer at a time.

##Usage
The control buttons are found in the main container (nVoid_AE_kf_importer) under the 'Settings' heading.
The 4 parameters are 'COMP Name', 'File Name' and 'Frame Length', and 'Create'. 'COMP Name is what your new Animation COMP will be named. 'File Name' is the file that contains the text-form After Effects keyframe information. 'Frame Length is the length of the animation that will created. 'Create' creates and initializes the new Animation COMP.

##Example
#After Effects :
- 


##Troubleshooting:
If you find an issue, submit a pull request or post an issue on this repo. 

##Attribution

If you use this in one of your projects, feel free to give us (nVoid) a shoutout or just let us know what you're up to! 
