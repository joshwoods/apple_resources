

- ARKit
-  ARSKViewDelegate 

Protocol

# ARSKViewDelegate

Methods you can implement to mediate the automatic synchronization of SpriteKit content with an AR session.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
protocol ARSKViewDelegate : ARSessionObserver, SKViewDelegate
```

## Overview

Implement this protocol to provide SpriteKit content corresponding to ARAnchor objects tracked by the view’s AR session, or to manage the view’s automatic updating of such content.

This protocol extends the ARSessionObserver protocol, so your session delegate can also implement those methods to respond to changes in session status.

## Topics

### Handling Content Updates

func view(ARSKView, nodeFor: ARAnchor) -> SKNode?

Asks the delegate to provide a SpriteKit node corresponding to a newly added anchor.

func view(ARSKView, didAdd: SKNode, for: ARAnchor)

Tells the delegate that a SpriteKit node corresponding to a new AR anchor has been added to the scene.

func view(ARSKView, willUpdate: SKNode, for: ARAnchor)

Tells the delegate that a SpriteKit node’s properties will be updated to match the current state of its corresponding anchor.

func view(ARSKView, didUpdate: SKNode, for: ARAnchor)

Tells the delegate that a SpriteKit node’s properties have been updated to match the current state of its corresponding anchor.

func view(ARSKView, didRemove: SKNode, for: ARAnchor)

Tells the delegate that the SpriteKit node corresponding to an AR anchor has been removed from the scene.

## Relationships

### Inherits From

- ARSessionObserver
- NSObjectProtocol
- SKViewDelegate

## See Also

### Responding to AR Updates

var delegate: (any ARSKViewDelegate)?

An object you provide to mediate synchronization of the view’s AR scene information with SpriteKit content.

