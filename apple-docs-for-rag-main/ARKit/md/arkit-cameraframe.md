

- ARKit
-  CameraFrame 

Structure

# CameraFrame

The representation of a camera frame.

visionOS 2.0+

``` source
struct CameraFrame
```

## Topics

### Getting camera frame information

var primarySample: CameraFrame.Sample

Gets the primary frame sample for a camera frame.

struct Sample

Information that describes a sample from a camera frame.

func sample(for: CameraFrameProvider.CameraPosition) -> CameraFrame.Sample?

Returns the camera frame sample for a given camera position.

var description: String

A textual representation of this camera frame.

## Relationships

### Conforms To

- CustomStringConvertible
- Equatable
- Sendable

## See Also

### Camera sampling

class CameraFrameProvider

An object that provides camera streams.

struct CameraVideoFormat

A structure that represents a camera video format.

