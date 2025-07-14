

- ARKit
- ARTrackable
-  isTracked 

Instance Property

# isTracked

A Boolean value that indicates whether the object’s transform is valid.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
var isTracked: Bool { get }
```

**Required**

## Discussion

If this value is true, the object’s transform currently matches the position and orientation of the real-world object it represents.

If this value is false, the object is not guaranteed to match the movement of its corresponding real-world feature, even if it remains in the visible scene.

