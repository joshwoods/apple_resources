

- UIKit
- UIShape
-  capsule 

Type Property

# capsule

Creates a capsule shape, a rounded rectangle with a corner radius equal to half the length of the rectangle’s smallest edge.

iOS 17.0+iPadOS 17.0+Mac CatalystvisionOS 1.0+

``` source
static var capsule: UIShape { get }
```

## See Also

### Creating a hover shape

static var rect: UIShape

Creates a rectangular shape.

static var circle: UIShape

Creates a circular shape, with a radius equal to half the length of the frame rectangle’s smallest edge.

static func rect(cornerRadius: CGFloat, cornerCurve: UICornerCurve, maskedCorners: UIRectCorner) -> UIShape

Creates a rectangular shape with rounded corners, using the provided corner radius, corner curve, and rectangle corners.

static func fixedRect(CGRect, cornerRadius: CGFloat, cornerCurve: UICornerCurve, maskedCorners: UIRectCorner) -> UIShape

Creates a fixed rectangular shape that uses the provided rectangle as its shape, regardless of the frame that contains it.

enum UICornerCurve

The corner curve to apply to a view.

