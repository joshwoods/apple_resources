

- Core Location
- CLHeading
-  trueHeading 

Instance Property

# trueHeading

The heading (measured in degrees) relative to true north.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.7+watchOS 2.0+

``` source
var trueHeading: CLLocationDirection { get }
```

## Discussion

The value in this property represents the heading relative to the geographic North Pole. The value `0` means the device is pointed toward true north, `90` means it is pointed due east, `180` means it is pointed due south, and so on. A negative value indicates that the heading could not be determined.

In iOS 3.x and earlier, the value in this property is always measured relative to the top of the device in a portrait orientation, regardless of the device’s actual physical or interface orientation. In iOS 4.0 and later, the value is measured relative to the heading orientation specified by the location manager. For more information, see the headingOrientation property in CLLocationManager.

Important

This property contains a valid value only if location updates are also enabled for the corresponding location manager object. Because the position of true north is different from the position of magnetic north on the Earth’s surface, Core Location needs the current location of the device to compute the value of this property.

## See Also

### Getting the heading values

var magneticHeading: CLLocationDirection

The heading (measured in degrees) relative to magnetic north.

var headingAccuracy: CLLocationDirection

The maximum deviation (measured in degrees) between the reported heading and the true geomagnetic heading.

