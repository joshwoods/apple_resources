

- Core Motion
- CMAltitudeData
-  relativeAltitude 

Instance Property

# relativeAltitude

The change in altitude (in meters) since the first reported event.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+watchOS 2.0+

``` source
var relativeAltitude: NSNumber { get }
```

## Discussion

For the first altitude event delivered to your altimeter object, the value of this property is `0`. Subsequent events contain a number that reflects the relative change in altitude with respect to the first reported event. For example, if the altitude changed five meters between the first and second events, the value in this property is `5` for the second event.

## See Also

### Getting the Altitude Data

var pressure: NSNumber

The recorded pressure, in kilopascals.

