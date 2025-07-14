

- MapKit
- MKDirections
- MKDirections.Response
-  source 

Instance Property

# source

The start point of the route.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
var source: MKMapItem { get }
```

## Discussion

The item in this property may contain additional details that aren’t in the original item you use to create the MKDirections.Request object.

## See Also

### Getting the end points

var destination: MKMapItem

The end point of the route.

