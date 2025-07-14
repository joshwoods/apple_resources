

- Core Location
-  kCLLocationAccuracyBest 

Global Variable

# kCLLocationAccuracyBest

The best level of accuracy available.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kCLLocationAccuracyBest: CLLocationAccuracy
```

## Discussion

Specify this constant when you want very high accuracy but don’t need the same level of accuracy required for navigation apps.

This level of accurate is available only if `isAuthorizedForPreciseLocation` is true.

## See Also

### Desired Accuracy Constants

let kCLLocationAccuracyBestForNavigation: CLLocationAccuracy

The highest possible accuracy that uses additional sensor data to facilitate navigation apps.

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

