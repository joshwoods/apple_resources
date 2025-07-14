

- StoreKit
- SKOverlay
-  SKOverlay.Position 

Enumeration

# SKOverlay.Position

Constants that identify the position of an overlay on the screen.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
enum Position
```

## Topics

### Describing the Overlay’s Position

case bottom

Specifies that the overlay is at the bottom of the screen.

case bottomRaised

Specifies that the overlay is at a raised position at the bottom of the screen.

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

### Creating an App Clip Configuration

init(position: SKOverlay.Position)

Creates an object that represents the attributes of an overlay you use to recommend an App Clip’s corresponding app.

var position: SKOverlay.Position

The position of the overlay on the screen.

