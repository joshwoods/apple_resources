

- SwiftUI
- ButtonBorderShape
-  capsule 

Type Property

# capsule

A capsule shape.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 8.0+

``` source
static let capsule: ButtonBorderShape
```

## Discussion

Use the buttonBorderShape(_:) view modifier to apply the shape to bordered buttons within a view hierarchy.

Note

This has no effect on non-widget system buttons in macOS.

## See Also

### Getting border shapes

static let automatic: ButtonBorderShape

A shape that defers to the system to determine an appropriate shape for the given context and platform.

static let circle: ButtonBorderShape

A circular shape.

static let roundedRectangle: ButtonBorderShape

A rounded rectangle shape.

static func roundedRectangle(radius: CGFloat) -> ButtonBorderShape

A rounded rectangle shape.

