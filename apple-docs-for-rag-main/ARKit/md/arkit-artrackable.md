

- ARKit
-  ARTrackable 

Protocol

# ARTrackable

An interface for objects that track the location of real-world objects or locations.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
protocol ARTrackable : NSObjectProtocol
```

## Overview

This protocol is adopted by ARKit classes, such as the ARFaceAnchor class, that represent moving objects in a scene.

ARKit automatically manages representations of such objects in an active AR session, ensuring that changes in the real-world object’s position and orientation (the transform property for anchors) are reflected in corresponding ARKit objects. The isTracked property indicates whether the current transform is valid with respect to movement of the real-world object.

Trackable anchor classes affect other ARKit behaviors:

- The getCurrentWorldMap(completionHandler:) method automatically includes only non-trackable anchors in the ARWorldMap it creates. (After you create a world map, you can add other anchors to it if you choose.)

- ARSCNView and ARSKView automatically hide the nodes for anchors whose isTracked property is false.

- World-tracking sessions use non-trackable anchors to optimize tracking quality in the area around each anchor. Trackable anchors do not affect world tracking.

## Topics

### Monitoring Tracking State

var isTracked: Bool

A Boolean value that indicates whether the object’s transform is valid.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- ARAppClipCodeAnchor
- ARBodyAnchor
- ARFaceAnchor
- ARGeoAnchor
- ARImageAnchor

## See Also

### Common Types

class ARAnchor

An object that specifies the position and orientation of an item in the physical environment.

protocol ARAnchorCopying

Support for custom anchor subclasses.

