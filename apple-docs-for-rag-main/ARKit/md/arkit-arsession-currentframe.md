

- ARKit
- ARSession
-  currentFrame 

Instance Property

# currentFrame

The most recent still frame captured by the active camera feed, including ARKit’s interpretation of it.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
@NSCopying
var currentFrame: ARFrame? { get }
```

## Mentioned in 

Displaying an AR Experience with Metal

## See Also

### Accessing the camera frame

class ARFrame

A video image captured as part of a session with position-tracking information.

func captureHighResolutionFrame(completion: (ARFrame?, (any Error)?) -> Void)

Requests a frame outside of the normal frequency that contains a high-resolution captured image.

