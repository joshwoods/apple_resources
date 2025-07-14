

- ARKit
-  ARSCNViewDelegate 

Protocol

# ARSCNViewDelegate

Methods you can implement to mediate the automatic synchronization of SceneKit content with an AR session.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
protocol ARSCNViewDelegate : ARSessionObserver, SCNSceneRendererDelegate
```

## Mentioned in 

Providing 3D Virtual Content with SceneKit

## Overview

Implement this protocol to provide SceneKit content corresponding to ARAnchor objects tracked by the view’s AR session, or to manage the view’s automatic updating of such content.

This protocol extends the ARSessionObserver protocol, so your session delegate can also implement those methods to respond to changes in session status.

## Topics

### Handling Content Updates

func renderer(any SCNSceneRenderer, nodeFor: ARAnchor) -> SCNNode?

Asks the delegate to provide a SceneKit node corresponding to a newly added anchor.

func renderer(any SCNSceneRenderer, didAdd: SCNNode, for: ARAnchor)

Tells the delegate that a SceneKit node corresponding to a new AR anchor has been added to the scene.

func renderer(any SCNSceneRenderer, willUpdate: SCNNode, for: ARAnchor)

Tells the delegate that a SceneKit node’s properties will be updated to match the current state of its corresponding anchor.

func renderer(any SCNSceneRenderer, didUpdate: SCNNode, for: ARAnchor)

Tells the delegate that a SceneKit node’s properties have been updated to match the current state of its corresponding anchor.

func renderer(any SCNSceneRenderer, didRemove: SCNNode, for: ARAnchor)

Tells the delegate that the SceneKit node corresponding to a removed AR anchor has been removed from the scene.

## Relationships

### Inherits From

- ARSessionObserver
- NSObjectProtocol
- SCNSceneRendererDelegate

## See Also

### Responding to AR Updates

var delegate: (any ARSCNViewDelegate)?

An object you provide to mediate synchronization of the view’s AR scene information with SceneKit content.

