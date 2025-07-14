

- ARKit
-  ARSessionDelegate 

Protocol

# ARSessionDelegate

Methods you can implement to receive captured video frame images and tracking state from an AR session.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
protocol ARSessionDelegate : ARSessionObserver
```

## Overview

Implement this protocol if you need to work directly with ARFrame objects captured by the session or directly follow changes to the session’s set of tracked ARAnchor objects. Typically, you adopt this protocol when building a custom view for displaying AR content—if you display content with SceneKit or SpriteKit, the ARSCNViewDelegate and ARSKViewDelegate protocols provide similar information and integrate with those technologies.

This protocol extends the ARSessionObserver protocol, so your session delegate can also implement those methods to respond to changes in session status.

## Topics

### Receiving Camera Frames

func session(ARSession, didUpdate: ARFrame)

Provides a newly captured camera image and accompanying AR information to the delegate.

### Handling Content Updates

func session(ARSession, didAdd: [ARAnchor])

Tells the delegate that one or more anchors have been added to the session.

func session(ARSession, didUpdate: [ARAnchor])

Tells the delegate that the session has adjusted the properties of one or more anchors.

func session(ARSession, didRemove: [ARAnchor])

Tells the delegate that one or more anchors have been removed from the session.

## Relationships

### Inherits From

- ARSessionObserver
- NSObjectProtocol

## See Also

### Responding to events

var delegate: (any ARSessionDelegate)?

An object you provide to receive captured video images and tracking information, or to respond to changes in session status.

var delegateQueue: dispatch_queue_t?

The dispatch queue through which the session calls your delegate methods.

protocol ARSessionObserver

Methods you can implement to respond to changes in the state of an AR session.

