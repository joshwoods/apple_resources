

- AppKit
- NSBezierPath
-  contains(\_:) 

Instance Method

# contains(\_:)

Returns a Boolean value that indicates whether the path contains the specified point.

macOS

``` source
func contains(_ point: NSPoint) -> Bool
```

## Parameters 

`point`  

The point to test against the path, specified in the path object’s coordinate system.

## Return Value

true if the path’s enclosed area contains the specified point; otherwise, false.

## Discussion

This method checks the point against the path itself and the area it encloses. When determining hits in the enclosed area, this method uses the non-zero winding rule (NSNonZeroWindingRule). It does not take into account the line width used to stroke the path.

