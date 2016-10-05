# TouchDesigner-AE-Import
TouchDesigner088 component that imports keyframes from an After Effects layer exported into a text file.

## Build and Version
This tool requires 'Custom Parameters' functionality within TouchDesigner (Build 45000 and above). It was created, and is stable, in 64-bit build 61480.

## Installation
Add the ```nVoid_AE_keyframe_importer.tox``` component into your project.

## Usage
The control buttons are found as custom parameters on the component ```nVoid_AE_kf_importer.tox``` under the ```Settings``` parameter page. The 4 parameters are ```COMP Name```, ```File Name``` and ```Frame Length```, and ```Create```. ```COMP Name``` is what your new Animation COMP will be named. ```File Name``` is the file that contains the text-form After Effects keyframe information. ```Default Curve Function``` allows you to choose the default easing function for keyframes that don't have one specified. ```Frame Length``` is the length of the animation that will created. ```Create``` creates and initializes the new Animation COMP.

## Example Usage

### In After Effects
1) Click and drag to select all the keyframes that are located on one layer of an After Effect Composition. Keyframes will become blue when they have been successfully selected. *NOTE*: If you try to select keyframes in more than one layer you will get the message ```After Effects must have keyframes selected from one layer in order to export them as text```. 

2) Go to the ```Edit``` menu and select ```Copy```, or press CONTROL + C to copy the keyframe data. 

3) Open your text editor of choice, and paste (CONTROL + V) the keyframe data.

4) Save the file as a ```.txt``` file

### In TouchDesigner
1) In the ```COMP Name``` text box, enter the name you would like the new Animation COMP to be called, for example ```HelloAnimation```

2) In the ```File Name``` text box, enter the full path to the text file that contains your keyframe data, or use the ```+``` button on the right to navigate to it.

3) In the ```Frame Length``` parameter, set the length of your animation in frames.

4) Hit the ```Create``` pulse button and your new Animation COMP will appear to the right of the ```nVoid_AE_kf_importer``` component.

## Notes about After Effects
### Copying Keyframes :
Keyframes can only be converted to text from one layer at a time. Do not copy and paste multiple layers of keyframe data into a single text file, that is currently not supported.

*Tip : *

To keep all keyframes on a single layer, you can use ```control layers``` with ```expression controls```, which are referenced by the other layers in the project. (Thanks to Hal Lovemelt for providing the AE demo that is included in the package)

This video explains ```control layers``` in more depth :
(https://youtu.be/YQdlWD-b6Cg)

### Curves
Interpolation methods and curves (i.e. linear, gaussian, ease-in ease-out) aren't available data points when exporting After Effects layer keyframe data into a text file, so you will need to adjust the interpolation methods between keyframes manually in the Animation COMP editor after you import the keyframe values. 

## Troubleshooting:
If you find an issue, submit a pull request or post an issue on this repo. 

## Attribution
If you use this in one of your projects, feel free to give us (nVoid) a shoutout or just let us know what you're up to! 
