

- SwiftUI
- ButtonBorderShape
-  roundedRectangle 

Type Property

# roundedRectangle

A rounded rectangle shape.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static let roundedRectangle: ButtonBorderShape
```

## Discussion

Use the buttonBorderShape(_:) view modifier to apply the shape to bordered buttons within a view hierarchy.

## See Also

### Getting border shapes

static let automatic: ButtonBorderShape

A shape that defers to the system to determine an appropriate shape for the given context and platform.

static let capsule: ButtonBorderShape

A capsule shape.

static let circle: ButtonBorderShape

A circular shape.

static func roundedRectangle(radius: CGFloat) -> ButtonBorderShape

A rounded rectangle shape.

