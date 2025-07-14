

- MapKit
- MKPolylineRenderer
-  strokeStart 

Instance Property

# strokeStart

The unit distance along the line where the stroke starts.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var strokeStart: CGFloat { get set }
```

## Discussion

Use this property and strokeEnd to render a portion of the line. Use location(atPointIndex:) to get unit distance locations for point indices along the line.

## See Also

### Accessing the stroke

var strokeEnd: CGFloat

The unit distance along the line where the stroke ends.

