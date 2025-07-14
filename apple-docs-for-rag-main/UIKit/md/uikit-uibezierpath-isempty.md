

- UIKit
- UIBezierPath
-  isEmpty 

Instance Property

# isEmpty

A Boolean value that indicates whether the path has any valid elements.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var isEmpty: Bool { get }
```

## Discussion

Valid path elements include commands to move to a specified point, draw a line or curve segment, or close the path. Thus, a path is not considered empty even if all you do is call the move(to:) method.

## See Also

### Performing hit-testing

func contains(CGPoint) -> Bool

Returns a Boolean value that indicates whether the specified point is within the region that the path encloses.

var bounds: CGRect

The bounding rectangle of the path.

