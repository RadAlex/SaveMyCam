# SaveMyCam
Plugin for Unreal Engine that implements pilot actor undo/redo issue. So you never ruin your perfect view again!

## How to install
1. Get the plugin on Fab
2. In Epic Games launcher, open Library tab, find SaveMyCamera plugin under Fab Library section.
3. Press install to engine, choose your engine version and install
4. If plugin is not enabled: Go to Edit -> Plugins -> In search field type "Save My Camera", tick checkbox to install and restart engine, if prompted

## In case you are installing using source
1. Create a project, or use existing
2. Copy "SaveMyCam" folder into "Plugins" folder (create if needed)
3. If it is already a C++ project, generate project files and build your project
4. If not, just start the project and build SaveMyCam module when prompted

## How to use
1. Add a camera to your scene
2. Start piloting your camera by choosing the camera actor under Camera options menu in desired viewport
<img width="472" height="246" alt="image" src="https://github.com/user-attachments/assets/b0696125-168d-4055-b99a-1697afce5ddc" />

or by right clicking in scene tree and choosing pilot this actor
<img width="691" height="364" alt="image" src="https://github.com/user-attachments/assets/b7a5506e-5da9-4c93-850e-dfb6d8bda67b" />


## **!!!Important!!! For undo/redo to take effect you need to move or rotate piloted actor at least once!**


### For Unreal 5.6 and up
While still piloting actor, in viewport toolbar you will see 2 buttons near Camera label (Perspective by default) 
<img width="390" height="82" alt="image" src="https://github.com/user-attachments/assets/3872c80f-e355-41c9-abf2-2104b85a2206" />

Press left to Undo, right to Redo

### For Unreal 5.5 and lower
Open viewport toolbar Options menu, Undo and Redo buttons are located under Pilot history subsection 
<img width="360" height="792" alt="image" src="https://github.com/user-attachments/assets/31fee153-3a82-423a-9a8e-a7304d84c232" />

Some might ask, why wouldn't you expose it in Camera menu instead? Well, prior 5.5 Unreal doesn't expose viewport context from that menu, dunno why (there definitely should be some logic behind it, although I fail to grasp it). If you have a custom engine build, there is a way to move it to Camera menu, contact me if needed.

# Questions
1. **Can I pilot a broom?** Sure, you can pilot anything that is a derivative of AActor, light, box, etc. It will record movement with no hassle.
2. **I have stopped piloting!!! Please help! I need to undo!** Do not fret, history is still there as long as you don't close the engine. Just start piloting again and undo/redo.
