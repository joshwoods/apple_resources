

- MapKit
- MKCoordinateSpan
-  longitudeDelta 

Instance Property

# longitudeDelta

The amount of east-to-west distance (measured in degrees) to display for the map region.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var longitudeDelta: CLLocationDegrees
```

## Discussion

The number of kilometers spanned by a longitude range varies based on the current latitude. For example, one degree of longitude spans a distance of approximately 111 kilometers (69 miles) at the equator but shrinks to 0 kilometers at the poles.

## See Also

### Getting the span coordinates

var latitudeDelta: CLLocationDegrees

The amount of north-to-south distance (measured in degrees) to display on the map.

