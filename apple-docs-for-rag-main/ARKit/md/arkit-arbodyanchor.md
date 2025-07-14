

- ARKit
-  ARBodyAnchor 

Class

# ARBodyAnchor

An anchor that tracks the position and movement of a human body in the rear-facing camera.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
class ARBodyAnchor
```

## Overview

This ARAnchor subclass tracks the movement of a single person. You enable body tracking by running your session using ARBodyTrackingConfiguration.

When ARKit recognizes a person in the back camera feed, it calls your delegate’s session(_:didAdd:) function with ARBodyAnchor. A body anchor’s transform position defines the world position of the body’s hip joint.

You can also check within the frame’s anchors for a body that ARKit is tracking.

### Place a Skeleton on a Surface

Because a body anchor’s origin maps to the hip joint, you calculate the current offset of the feet to the hip to place the body’s skeleton on a surface. By passing the foot joint index to jointModelTransforms, you get the foot’s offset from skeleton’s origin.

```
static var hipToFootOffset: Float {
    // Get an index for a foot. 
    let footIndex = ARSkeletonDefinition.defaultBody3D.index(forJointName: .leftFoot)
    // Get the foot's world-space offset from the hip. 
    let footTransform = ARSkeletonDefinition.defaultBody3D.neutralBodySkeleton3D!.jointModelTransforms[footIndex]
    // Return the height by getting just the y-value. 
    let distanceFromHipOnY = abs(footTransform.columns.3.y) 
    return distanceFromHipOnY
}
```

## Topics

### Interpreting 3D Motion

var skeleton: ARSkeleton3D

The tracked body in 3D.

### Getting Scale Information

var estimatedScaleFactor: CGFloat

A factor that relates the body’s default height with the height ARKit estimates at runtime.

## Relationships

### Inherits From

- ARAnchor

### Conforms To

- ARAnchorCopying
- ARTrackable
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Body Position Tracking

Capturing Body Motion in 3D

Track a person in the physical environment and visualize their motion by applying the same body movements to a virtual character.

Rigging a Model for Motion Capture

Configure custom 3D models so ARKit’s human body-tracking feature can control them.

Validating a Model for Motion Capture

Verify that your character model matches ARKit’s Motion Capture requirements.

