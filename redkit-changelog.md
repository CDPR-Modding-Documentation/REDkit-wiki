---
description: >-
  All patches released for The Witcher 3 REDkit since its release. Last updated
  13 August 2025
---

# REDkit Changelog

[Back to Home](./)

### Patch 3

#### Features

**Scene Editor:**

* Double-clicking on an empty animation event will now open AnimBrowser.
* AnimBrowser will now open on double-click.
* Double-clicking on the timeline will now create an event for the clicked track. If it’s an animation, it will open the AnimBrowser.
* The "Swipe" button will now remove Scene Editor's subtitles as well.
* If there’s a Scene Editor fragment, it will always show the scene subtitles.
* All additional debug information will be displayed when the Scenes debug checkbox is enabled.
* Enabling Free Camera Mode will restore the editor's default camera FOV.
* Camera FOV in preview will not be editable.
* FOV in Free Camera Mode will always use the last free camera FOV setup.
* FOV on the viewport will now refresh when switching cameras in Edit Mode.
* Viewport FOV will apply to the active camera on change (the edited camera in Edit Mode or to the free camera in Free Mode).
* Fixed issues with the Undo Manager.

**Miscellaneous**

* Added an option to create .xml files in Asset Browser with correct encoding.
* The “World” tab will be updated with the current World name.
* Updated the Blender Plugin:
* Added pose bone weights for different NPCs, it can be selected during lipsync generation.
* Added interpolation easing while generating a lipsync.
* Fixed issues with installing the plugin on Blender 4.
* Updated the credits in the “About” section.
* Added shortcuts to move plane and select plane for the world edit gizmo (press X and Y to select the XY plane).
* Added a button to set default lipsync and audio overwrite paths in scenes.

#### Fixes

**Various UI fixes:**

* Fixed an issue where dragging panels in the Scene Editor would cause a crash.
* Fixed an issue where the editor would crash when loading a level while having a floating toolbar.
* Fixed an issue where the Item Select dialogue box would not close properly.
* The gizmo will now use thicker debug lines.
* Improved the check icon in the PropertyGrid.

**Various Scene Editor fixes:**

* Saving will now always teleport to the first node.
* Fixed a crash on deleting any pause event on Timeline.
* Fixed a Scene Editor crash when switching from Edit Camera Mode to Free Camera Mode and trying to edit the camera from the Properties page.

**Miscellaneous fixes:**

* Fixed an issue where the tangent calculator didn't work properly for some vertices during uncooking.
* Fixed an issue where the Vertex paint tool wouldn’t save changes.
* Fixed an issue where the .xml parser error would not show the correct file path.
* Fixed an issue where the minimap generation stretched output images.
* Fixed an issue where loading game definitions with standard templates would crash under certain conditions.
* Fixes for revert and drag-and-drop actions in Journal Editor.
* Fixed splash screen sizing for the game.
* Fixed an issue where the world edit gizmo could get stuck when pressing two shortcut keys.
* Updated the Wwise license acquisition steps.
* Fixed an issue where searching for a quest graph block by name criteria didn't work properly.

### Patch 2

* \[Experimental] Added an option to start the editor in dark mode (View → Settings → Editor Configuration → Editor → startInDarkMode).
* REDkit is now shipped with pre-generated thumbnails. Users can update them for checked-out and added assets.
* You can now use a .jpg image as a thumbnail when publishing a mod.
* Added an option to disable the automatic reopening of resource editors that were open when the editor was last closed.
* Added an option in Scene Editor to generate all misssing lipsync and voiceover. It will use Windows' text to speech feature for voiceover, lipsync generation is possible if the audio is generated and the \* Editor knows the location of the Blender Plugin.
* Added the languages that were missing after cooking strings.
* Added scrollbars for the "Entry Attributes" section in the Color tab in the Entity Editor.
* Added support for additional virtual directories. REDkit can now attach additional directories besides the uncook depot (read-only). Essentially, your mod project can now depend on another mod.
* Texture Viewer and Material Editor window layouts will now be saved.
* 3D gizmo handling will now interact correctly with the cursor.
* Added keyboard shortcuts for manipulating the gizmo. Shortcuts can be customized in "View" → "Customize editor shortcuts...".
* Set defaultPlayerTemplate defaultCameraTemplate when creating a new game resource definition.
* Hid some popups (e.g. New Game+ popup) that still appeared when playing from a .redgame definition.
* Using the "Tools" → "Generate missing unique script tags" option in Journal Editor will now properly fill out the missing unique script tag fields of new journal entries.
* Fixed issues with playback buttons in the Entity Editor.
* Editing multi-property values in Scene Editor by text will now be disabled instead of resulting in a crash.
* Implemented a material .xml metadata exporter/importer for Apex resources (CApexClothResource and CApexDestructionResource).
* Having the word "scripts" in the project name won't break script compilation anymore.
* Fixed the scaling of the "By Tag" editor window.
* Fixed description tooltips not always showing after hovering over a property field.
* Fixed an issue where recent projects could contain duplicates under certain conditions.
* Fixed an issue where when trying to save .w2mi files, the user was asked to "overwrite the existing file", although there was no file with the same name.
* Various fixes for the Journal Editor: removed non-functional elements, improved color coding, fixed checking-out and reverting.
* Added some fixes for importing scenes.
* Fixed some UI glitches in the Asset Browser.
* Several UI fixes for the PathLib Tool.
* Various stability improvements and crash fixes.

### Patch 1

* Fixed an issue where the cursor could disappear in the editor after zooming in in the preview in the Texture Viewer.
* Generated navmesh instance will now be properly loaded back after saving and re-opening the world.
* Color picker in the Environment Editor will now properly show colors.
* Creating a new world and generating terrain will no longer fail when Ray Tracing is enabled.
* Fixed the trajectory calculation of bone motion extraction when importing animations.
* Various stability improvements and crash fixes.
* Various UI improvements to the Welcome dialog box.
* Editor will now check the game version before starting and warn the user if it's outdated.
* Various language fixes and tweaks.
* Disabled some not working or console-related debug filters.
* Editor will now remember the configurations in the Welcome dialog box even if the app was closed before starting completely.
* Map file (editormap.json) generated from the REDkit executable will now be included in the bin folder.
* New worlds can now be created as DLC mods.
* Assigned better default values in setup for Terrain Edit Tools.
* Added some new icons in the UI.
* Removed unused Import and Export settings sections in the Terrain Edit Tool.
* Removed the redundant Animation Friend tool.
* Made w3fac and w3dyng files editable if REDkit config is active.
* Various fixes for publishing on Steam Workshop.
* Added new tutorials (including WitcherScript documentation) to the REDkit User Guide.
