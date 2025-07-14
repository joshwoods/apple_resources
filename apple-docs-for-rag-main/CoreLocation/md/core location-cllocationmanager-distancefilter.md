

- Core Location
- CLLocationManager
-  distanceFilter 

Instance Property

# distanceFilter

The minimum distance in meters the device must move horizontally before an update event is generated.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var distanceFilter: CLLocationDistance { get set }
```

## Mentioned in 

Getting the current location of a device

## Discussion

This location manager measures this relative to the previously delivered location. Specify the value kCLDistanceFilterNone to receive notifications for all movements. The default value of this property is kCLDistanceFilterNone.

Use this property only in conjunction with the Standard location services and not with the Significant-change or Visits services.

### Special Considerations

In iOS, this property is declared as `nonatomic`. In macOS, it is declared as `atomic`.

## See Also

### Specifying distance and accuracy

let CLLocationDistanceMax: CLLocationDistance

A constant indicating the maximum distance.

let kCLDistanceFilterNone: CLLocationDistance

A constant indicating that all movement should be reported.

typealias CLLocationDistance

A distance in meters from an existing location.

var desiredAccuracy: CLLocationAccuracy

The accuracy of the location data that your app wants to receive.

typealias CLLocationAccuracy

The accuracy of a geographical coordinate.

