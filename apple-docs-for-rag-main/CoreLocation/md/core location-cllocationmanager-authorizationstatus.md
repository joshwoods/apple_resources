

- Core Location
- CLLocationManager
-  authorizationStatus 

Instance Property

# authorizationStatus

The current authorization status for the app.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var authorizationStatus: CLAuthorizationStatus { get }
```

## Return Value

A value indicating whether the app is authorized to use location services.

## Mentioned in 

Requesting authorization to use location services

## Discussion

Check this value when the locationManagerDidChangeAuthorization(_:) delegate callback indicates that the authorization status has changed.

The system is guaranteed to call the delegate method with the app’s initial authorization state and all authorization status changes.

The system manages the authorization status of a given app according to several factors. Users must authorize the app to use location services explicitly, and location services must be enabled in Settings \> Privacy. See Choosing the Location Services Authorization to Request for more information.

## See Also

### Requesting authorization for location services

func requestWhenInUseAuthorization()

Requests the user’s permission to use location services while the app is in use.

func requestAlwaysAuthorization()

Requests the user’s permission to use location services regardless of whether the app is in use.

func requestTemporaryFullAccuracyAuthorization(withPurposeKey: String, completion: (((any Error)?) -> Void)?)

Requests permission to temporarily use location services with full accuracy and reports the results to the provided completion handler.

func requestTemporaryFullAccuracyAuthorization(withPurposeKey: String)

Requests permission to temporarily use location services with full accuracy.

enum CLAuthorizationStatus

Constants that indicate the app’s authorization to use location services.

NSLocationDefaultAccuracyReduced

A Boolean value that indicates whether the app requests reduced location accuracy by default.

NSLocationAlwaysAndWhenInUseUsageDescription

A message that tells the user why the app is requesting access to the user’s location information at all times.

