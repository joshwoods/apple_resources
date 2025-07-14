

- UIKit
- UIBezierPath
-  bounds 

Instance Property

# bounds

The bounding rectangle of the path.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var bounds: CGRect { get }
```

## Discussion

The value in this property represents the smallest rectangle that completely encloses all points in the path, including any control points for Bézier and quadratic curves.

## See Also

### Performing hit-testing

func contains(CGPoint) -> Bool

Returns a Boolean value that indicates whether the specified point is within the region that the path encloses.

var isEmpty: Bool

A Boolean value that indicates whether the path has any valid elements.

