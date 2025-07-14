

- RealityKit
- Reality Composer
-  Bringing a Reality Composer scene to life 

Article

# Bringing a Reality Composer scene to life

Add animation and handle user input by using behaviors, triggers, and actions.

## Overview

Users can interact with your *Reality Composer* scenes in a number of different ways without you having to explicitly code for them using Reality Composer’s behaviors. You can, for example, allow a user’s touch to affect objects in your scene, or let objects respond when the user moves close to them.

Reality Composer includes a number of behavior presets that let you easily add common forms of interactivity to your scene. You can also build your own custom behaviors or use a preset as a starting point for building more complex behaviors. For more information, see Building custom behaviors.

### Add a behavior preset

Reality Composer provides six behavior presets that simplify adding common forms of interactivity to your scenes. If any objects in your scene are selected when you add a behavior from a preset, the new behavior is automatically configured to affect the selected object or objects. This list describes each of the behavior presets:

Tap & Flip  
Causes one or more objects to animate by jumping up and spinning around in response to user taps

Tap & Play Sound  
Plays a sound in response to user taps

Tap & Add Force  
Applies a force to objects that simulate physics in response to user taps

Start Hidden  
Causes one or more objects to be invisible when the scene starts

Wait & Show  
Causes one or more objects to start as invisible, then become visible after a specified duration

Proximity & Jiggle  
Causes one or more objects to jiggle in response to the viewer getting close to it

To add a behavior preset to your scene, select the object or objects you want as the target of the behavior, tap the Behaviors button in the toolbar to bring up the Behaviors pane, then tap the plus button to reveal a popover that shows all of the available behavior presets as well as an option to create a custom behavior. Select a preset and Reality Composer adds a new behavior to your scene based on that preset. If, for example, you select an object and add the “Tap and Flip” behavior, a new behavior is added to your scene. This behavior is automatically configured so that the selected object flips over whenever a user taps it. To test the behavior, select the Play button in the toolbar, then tap the selected object.

### Rename a behavior

A newly added behavior is named “Behavior.” Immediately rename behaviors to reflect what they actually do. On an iOS device, press and hold the behavior’s name and select Rename from the menu that appears. On a Mac, select a behavior, and choose Rename from the Edit menu or press the Return key.

## See Also

### Behaviors

Building custom behaviors

Create custom behaviors to control objects in your scene.

Creating a Trigger

Define when and how a behavior fires.

Adding interactivity to behaviors

Define what a behavior does by using actions.

