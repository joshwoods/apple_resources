

- SpriteKit
- SKScene
-  Subclassing Scenes Versus Assigning a Delegate 

Article

# Subclassing Scenes Versus Assigning a Delegate

Use a scene delegate to share app logic across various scenes.

## Overview

Often, your app subclasses SKScene to deliver gameplay. Your subclass usually:

- Lays out initial scene content

- Defines app logic that runs every frame

- Implements responder methods to handle keyboard, mouse, or touch events

An alternative pattern is to assign a delegate that handles SKScene instead. For example, if you make the view controller the delegate for your scene, it can use multiple scenes that share the same SKSceneDelegate implementations. The view controller participates in event handling and so it can respond to user input also.

Important

On macOS, you need to set the window’s nextResponder to your app’s view controller because by default, the view is the first responder to user input events.

## See Also

### Configuring a Delegate

var delegate: (any SKSceneDelegate)?

A delegate to be called during the animation loop.

protocol SKSceneDelegate

Methods that, when implemented, allow any class to participate in the SpriteKit render loop callbacks.

