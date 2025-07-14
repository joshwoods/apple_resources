

- MapKit
- MKPolygon
-  interiorPolygons 

Instance Property

# interiorPolygons

The array of polygons that nest inside the enclosing polygon.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
var interiorPolygons: [MKPolygon]? { get }
```

## Discussion

When the screen renders a polygon, the renderer masks the area that any interior polygons occupy so they aren’t part of the polygon.

