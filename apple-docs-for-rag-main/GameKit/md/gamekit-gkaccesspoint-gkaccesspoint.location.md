

- GameKit
- GKAccessPoint
-  GKAccessPoint.Location 

Enumeration

# GKAccessPoint.Location

Specifies the corner of the screen to display the access point.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
enum Location
```

## Topics

### Corners

case bottomLeading

The lower-left corner of the screen.

case bottomTrailing

The lower-right corner of the screen.

case topLeading

The upper-left corner of the screen.

case topTrailing

The upper-right corner of the screen.

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

### Managing the location

var location: GKAccessPoint.Location

The corner of the screen to display the access point.

var frameInScreenCoordinates: CGRect

The frame of the access point in screen coordinates.

var parentWindow: UIWindow?

The window that contains the access point.

