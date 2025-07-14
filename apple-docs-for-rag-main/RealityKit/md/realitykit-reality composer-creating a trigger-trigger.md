

- RealityKit
- Reality Composer
-  Creating a Trigger 

Article

# Creating a Trigger

Define when and how a behavior fires.

## Overview

Reality Composer supports five types of triggers: Tap, Scene Start, Proximity To Camera, Collide, and Notification. In Reality Composer’s Behavior pane, you click or tap inside the dashed box representing a trigger to specify the set of conditions or events that cause that trigger’s behavior to fire.

### Respond to taps and touches

Select the Tap trigger when you want a behavior to fire in response to the user tapping a specific object or objects. After adding a tap trigger to the behavior, select the object or objects in your scene that you want the user to interact with. If you accidentally select an object that you don’t want, click or tap it a second time to deselect it. When you’re finished making your selection, press the Done button. To make further changes to the affected objects, press the Choose button to return to selection mode.

Tip

You can only use tap triggers for detecting single taps with one finger. To detect more complex scenarios, such as double-taps, long presses, or multiple-finger taps, use a notification trigger and then use Gesture Recognizers or SwiftUI gesture detection. For more information, see Fire a behavior from code.

### Fire a behavior immediately

Select the Scene Start trigger if you want a behavior to fire as soon as your scene is loaded and displayed to the user. You would commonly used this type of trigger to set the starting state; for example, to hide objects you don’t want visible at first, or to initiate animations to run immediately.

### Fire behaviors when the user is near an object

Select the Proximity To Camera trigger if you want a behavior to fire whenever the camera—and, therefore, the user—gets close to specific objects in your scene. Specify how close the user must get by using the Distance slider on the trigger. If you then select the trigger, a green sphere is displayed around the affected objects to represent the specified distance. You can also drag the sphere to change the distance visually.

### Respond to object collisions

Select the Collide trigger if you want a behavior to fire whenever specific objects collide with other objects in your scene, or when objects collide with detected real-world surfaces.

Note

The target of a collide trigger must participate in your scene’s physics simulation. If you select an object that does not participate, Reality Composer prompts you to enable it.

### Fire a behavior from code

Select a Notification trigger to fire a behavior from code you write in Xcode. Notification triggers are a good option when none of the other trigger types meet your needs. When you create a notification trigger, Xcode automatically generates the code needed to activate the behavior.

To trigger a notification, call the `post()` function on the generated notification. If, for example, your scene has a Notification trigger called `SpinBox`, as shown in the figure below, trigger that behavior from your code like this:

```
myScene.notifications.spinBox.post() 
```

## See Also

### Behaviors

Bringing a Reality Composer scene to life

Add animation and handle user input by using behaviors, triggers, and actions.

Building custom behaviors

Create custom behaviors to control objects in your scene.

Adding interactivity to behaviors

Define what a behavior does by using actions.

