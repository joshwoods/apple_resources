

- Core Location
- CLVisit
-  horizontalAccuracy 

Instance Property

# horizontalAccuracy

The horizontal accuracy (in meters) of the specified coordinate.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.15+

``` source
var horizontalAccuracy: CLLocationAccuracy { get }
```

## Discussion

The latitude and longitude specified by the coordinate property identify the center of the circle, and this value indicates the radius of that circle.

## See Also

### Getting the location

var coordinate: CLLocationCoordinate2D

The geographical coordinate information.

