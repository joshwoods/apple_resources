

- MapKit
- MKAnnotationView
-  MKAnnotationView.CollisionMode 

Enumeration

# MKAnnotationView.CollisionMode

Constants that indicates how to interpret the collision frame rectangle of an annotation view.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
enum CollisionMode
```

## Topics

### Enumeration Cases

case rectangle

A constant that indicates that the annotation view uses the full collision frame rectangle for detecting collisions.

case circle

A constant that indicates that the annotation view uses an inscribed circle in the collision frame rectangle to determine collisions.

case none

A constant indicating that collisions can’t occur.

case rectangle

A constant that indicates that the annotation view uses the full collision frame rectangle for detecting collisions.

case circle

A constant that indicates that the annotation view uses an inscribed circle in the collision frame rectangle to determine collisions.

case none

A constant indicating that collisions can’t occur.

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

### Managing collisions between annotation views

var collisionMode: MKAnnotationView.CollisionMode

The collision mode to use when interpreting the collision frame rectangle.

