

- SceneKit
-  SCNCameraProjectionDirection 

Enumeration

# SCNCameraProjectionDirection

Options for the axis used to determine field of view or orthographic projection.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
enum SCNCameraProjectionDirection
```

## Topics

### Projection Directions

case vertical

The camera’s field of view or orthographic scale are measured vertically.

case horizontal

The camera’s field of view or orthographic scale are measured horizontally.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Managing Field of View

var fieldOfView: CGFloat

The vertical or horizontal viewing angle of the camera.

var focalLength: CGFloat

The camera’s focal length, in millimeters.

var sensorHeight: CGFloat

The vertical size of the camera’s imaging plane, in millimeters.

var projectionDirection: SCNCameraProjectionDirection

The axis used to determine field of view or orthographic scale.

