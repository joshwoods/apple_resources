

- ARKit
- ARPlaneAnchor
-  ARPlaneAnchor.Alignment 

Enumeration

# ARPlaneAnchor.Alignment

The kinds of alignment — horizontal or vertical — that a plane anchor can have.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
enum Alignment
```

## Topics

### Alignment Values

case horizontal

The plane is perpendicular to gravity.

case vertical

The plane is parallel to gravity.

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

### Orientation

var alignment: ARPlaneAnchor.Alignment

The general orientation of the detected plane with respect to gravity.

