

- UIKit
- NSStringDrawingContext
-  totalBounds 

Instance Property

# totalBounds

The most recent bounding rectangle that the system used to draw the string.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var totalBounds: CGRect { get }
```

## Discussion

This property contains the bounding rectangle that was last used when calling the draw(with:options:context:) method. The rectangle is specified in the coordinate system of the drawn string. (The origin of the bounds corresponds to neither a view the string might have been drawn into nor the origin of a possible draw(in:) call.)

