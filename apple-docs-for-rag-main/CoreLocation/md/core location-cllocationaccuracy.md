

- Core Location
-  CLLocationAccuracy 

Type Alias

# CLLocationAccuracy

The accuracy of a geographical coordinate.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
typealias CLLocationAccuracy = Double
```

## Discussion

When reported in a CLLocation object, accuracy values are the number of meters from the original geographic coordinate that could yield the user’s actual location. When specifying values for the desiredAccuracy property of your CLLocationManager object, use one of the appropriate constants.

## Topics

### Desired Accuracy Constants

let kCLLocationAccuracyBestForNavigation: CLLocationAccuracy

The highest possible accuracy that uses additional sensor data to facilitate navigation apps.

let kCLLocationAccuracyBest: CLLocationAccuracy

The best level of accuracy available.

let kCLLocationAccuracyNearestTenMeters: CLLocationAccuracy

Accurate to within ten meters of the desired target.

let kCLLocationAccuracyHundredMeters: CLLocationAccuracy

Accurate to within one hundred meters.

let kCLLocationAccuracyKilometer: CLLocationAccuracy

Accurate to the nearest kilometer.

let kCLLocationAccuracyThreeKilometers: CLLocationAccuracy

Accurate to the nearest three kilometers.

let kCLLocationAccuracyReduced: CLLocationAccuracy

The level of accuracy used when an app isn’t authorized for full accuracy location data.

## See Also

### Getting the location accuracy

var horizontalAccuracy: CLLocationAccuracy

The radius of uncertainty for the location, measured in meters.

var verticalAccuracy: CLLocationAccuracy

The validity of the altitude values, and their estimated uncertainty, measured in meters.

