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
*###After Effects :*

- Click and drag to select all the keyframes that are located on one layer. (If you try to select keyframes in more than one layer you will get the message 'After Effects must have keyframes selected from one layer in order to export them as text' once you try to paste them.) Keyframes will become blue when they have been successfully selected

- Go to the EDIT menu, or press CONTROL + C to copy the keyframe data. 

- Open your text editor of choice, and paste (CONTROL + V) the keyframe data.

- Save the text file.

*###TouchDesigner :*

- 


##Troubleshooting:
If you find an issue, submit a pull request or post an issue on this repo. 

##Attribution

If you use this in one of your projects, feel free to give us (nVoid) a shoutout or just let us know what you're up to! 
