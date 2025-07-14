

- TVUIKit
-  TVCaptionButtonViewMotionDirection 

Enumeration

# TVCaptionButtonViewMotionDirection

The directions that the caption button view can tilt in response to user interactions on the remote.

tvOS 12.0+

``` source
enum TVCaptionButtonViewMotionDirection
```

## Topics

### Tilt Directions

case all

The caption button view can tilt in all directions.

case horizontal

The caption button view can tilt in the horzontal direction.

case none

The caption button view can’t tilt.

case vertical

The caption button view can tilt in the vertical direction.

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

### Setting the Motion Direction

var motionDirection: TVCaptionButtonViewMotionDirection

The direction that the caption button view tilts in response to user interaction on the remote.

