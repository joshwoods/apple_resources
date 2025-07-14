

- Core Motion
- CMOdometerData
-  speedAccuracy 

Instance Property

# speedAccuracy

The accuracy of the speed value.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 10.15+visionOS 1.0+watchOS 10.0+

``` source
var speedAccuracy: CLLocationSpeedAccuracy { get }
```

## Discussion

This property measures the accuracy of the speed property. When this property contains `0` or a positive number, the value in the `speed` property is plus or minus the specified number of meters per second. When this property contains a negative number, the value in the `speed` property is invalid.

## See Also

### Getting the location accuracy

var verticalAccuracy: CLLocationAccuracy

The validity of the altitude values and their estimated uncertainty, measured in meters.

var deltaDistanceAccuracy: CLLocationAccuracy

The accuracy of the change in distance value.

