# THIS IS NOT FINISHED. THERE IS AN ISSUE WITH INPUT FORWARDING (ONLY MOUSE EVENTS ARE RECOGNIZED) WHICH LEAD TO VERY STRANGE BEHAVIOR.
If you're ndee85, feel free to base any porting efforts on this, however, as it does mostly work outside of the above issues.
Look into `_input()` and `forward_canvas_gui_input()` to fix this. (Also a note to self.)

# Asset Dropper - Godot Plugin
Asset Dropper is a plugin for Godots AssetLib. It provides tools to create a fast workflow for 2D level creation.

# Installation
Copy the addon directory into your godot project and then enable the plugin under "Project Settings -> Plugins"

#Usage
Global Shortcuts (Shortcuts that can be used directly in the 2D Editor)
 - A -> will preview the to be dropped/drawn node (make sure to create a Asset Group first)
 - Ctrl + 0-9 -> will create an Asset Group of all selected nodes
 - Shift + 0-9 -> will append selected nodes to existing Asset Groups
 - 0-9 -> will select the asset group
 - S -> opens the settings Popup
 - T -> set selected node as target node where all assets will be parented to (if not set, nodes will be placed where its instances are)
 
Preview Shortcuts (Shortcuts that can only be used when the preview is shown (A pressed))
 - F -> flip Asset horizontally
 - G -> flip Asset vertically
 - Left Mouse -> drop/draw Assset (based on the draw mode that is used)
 - Left Mouse + X -> constraint scaling to x axis
 - Left Mouse + Y -> constraint scaling to y axis
 