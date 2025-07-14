

- ARKit
-  ARAnchorCopying 

Protocol

# ARAnchorCopying

Support for custom anchor subclasses.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
protocol ARAnchorCopying : NSCopying
```

## Overview

An ARAnchor (or an instance of any anchor subclass) represents a position and orientation in world space, and optionally associates extra information with that point (like a name, or plane or image detection data). Each time ARKit generates an ARFrame object (describing the current environment as of a specific frame of live camera video), ARKit updates the anchors associated with the session as of that moment. Because anchor objects are immutable, ARKit must copy them to make changes from one ARFrame to the next.

If you create your own ARAnchor subclass, you must implement the init(anchor:) initializer required by this protocol. To ensure that any custom information in your subclass is maintained between successive frames, your implementation should copy any custom properties it declares.

## Topics

### Copying Anchors

init(anchor: ARAnchor)

Initializes a new anchor by copying custom information from another anchor.

**Required**

## Relationships

### Inherits From

- NSCopying

### Conforming Types

- ARAnchor
- ARAppClipCodeAnchor
- ARBodyAnchor
- AREnvironmentProbeAnchor
- ARFaceAnchor
- ARGeoAnchor
- ARImageAnchor
- ARMeshAnchor
- ARObjectAnchor
- ARParticipantAnchor
- ARPlaneAnchor

## See Also

### Common Types

class ARAnchor

An object that specifies the position and orientation of an item in the physical environment.

protocol ARTrackable

An interface for objects that track the location of real-world objects or locations.

