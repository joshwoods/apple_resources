

- MapKit
- MKPolygonRenderer
-  strokeEnd 

Instance Property

# strokeEnd

The unit distance along the polygon where the stroke ends.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var strokeEnd: CGFloat { get set }
```

## Discussion

Use this property and strokeStart to render a portion of the polygon. Use location(atPointIndex:) to get unit distance locations for point indices along the polygon.

## See Also

### Accessing the stroke

var strokeStart: CGFloat

The unit distance along the polygon where the stroke starts.

