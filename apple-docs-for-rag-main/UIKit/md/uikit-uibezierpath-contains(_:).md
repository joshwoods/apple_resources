

- UIKit
- UIBezierPath
-  contains(\_:) 

Instance Method

# contains(\_:)

Returns a Boolean value that indicates whether the specified point is within the region that the path encloses.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func contains(_ point: CGPoint) -> Bool
```

## Parameters 

`point`  

The point to test against the path, specified in the path object’s coordinate system.

## Return Value

true if the point is considered to be within the path’s enclosed area or false if it is not.

## Discussion

The receiver contains the specified point if that point is in a portion of a closed subpath that would normally be painted during a fill operation. This method uses the value of the usesEvenOddFillRule property to determine which parts of the subpath would be filled.

A point is not considered to be enclosed by the path if it is inside an open subpath, regardless of whether that area would be painted during a fill operation. Therefore, to determine mouse hits on open paths, you must create a copy of the path object and explicitly close any subpaths (using the close() method) before calling this method.

## See Also

### Performing hit-testing

var isEmpty: Bool

A Boolean value that indicates whether the path has any valid elements.

var bounds: CGRect

The bounding rectangle of the path.

