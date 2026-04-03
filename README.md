# Mr Mannequin Tools - Blender 5 Fix

This repository contains a modified version of the **Mr Mannequin Tools** addon to fix compatibility issues with Blender 5.

## Background
The original addon was last updated in 2022 and was mainly used with Blender 4.x.  
When using Blender 5, the addon failed during FBX export due to changes in the animation API.

## What was changed
The addon previously accessed animation data directly at the object level.  
In Blender 5, animation data is organized differently, requiring iteration through layers and channels.

The relevant parts of the code were updated to match the new API behavior.

## Current Status
- FBX export works without errors in Blender 5  
- The exported animation works in Unreal Engine, but may require adjusting import/settings  

## Installation
1. Download this repository as a ZIP  
2. Open Blender  
3. Go to: Edit → Preferences → Add-ons  
4. Click "Install" and select the addon folder or ZIP  
5. Enable the addon  

## Feedback
If you try this fix, feel free to open an issue or share feedback.  
It would help confirm compatibility and improve the addon.

## Notes
This was my first experience debugging and fixing an issue in a real-world addon.