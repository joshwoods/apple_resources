

- UIKit
- UIBezierPath
-  addClip() 

Instance Method

# addClip()

Uses the clipping path of the current graphics context to intersect the region that the path encloses, and makes the resulting shape the current clipping path.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func addClip()
```

## Discussion

This method modifies the visible drawing area of the current graphics context. After calling it, subsequent drawing operations result in rendered content only if they occur within the fill area of the specified path.

Important

If you need to remove the clipping region to perform subsequent drawing operations, you must save the current graphics state (using the saveGState() function) before calling this method. When you no longer need the clipping region, you can then restore the previous drawing properties and clipping region using the restoreGState() function.

The usesEvenOddFillRule property is used to determine whether the even-odd or non-zero rule is used to determine the area enclosed by the path.

