

- Core Location
- CLLocationManager
-  requestTemporaryFullAccuracyAuthorization(withPurposeKey:) 

Instance Method

# requestTemporaryFullAccuracyAuthorization(withPurposeKey:)

Requests permission to temporarily use location services with full accuracy.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
func requestTemporaryFullAccuracyAuthorization(withPurposeKey purposeKey: String)
```

## Parameters 

`purposeKey`  

A key in the NSLocationTemporaryUsageDescriptionDictionary dictionary of the app’s `Info.plist` file. The value for this key is an app-provided string that describes the reason for accessing location data with full accuracy. To localize a usage description, add an entry to your `InfoPlist.strings` file with the same key you provide for this parameter.

## Discussion

This method behaves the same as calling the requestTemporaryFullAccuracyAuthorization(withPurposeKey:completion:) method, passing `nil` as the completion closure. Use this method if your app’s logic to respond to changes in location data accuracy is already handled by the locationManagerDidChangeAuthorization(_:) delegate method, and your app doesn’t have any work to do in the closure.

## See Also

### Requesting authorization for location services

func requestWhenInUseAuthorization()

Requests the user’s permission to use location services while the app is in use.

func requestAlwaysAuthorization()

Requests the user’s permission to use location services regardless of whether the app is in use.

func requestTemporaryFullAccuracyAuthorization(withPurposeKey: String, completion: (((any Error)?) -> Void)?)

Requests permission to temporarily use location services with full accuracy and reports the results to the provided completion handler.

var authorizationStatus: CLAuthorizationStatus

The current authorization status for the app.

enum CLAuthorizationStatus

Constants that indicate the app’s authorization to use location services.

NSLocationDefaultAccuracyReduced

A Boolean value that indicates whether the app requests reduced location accuracy by default.

NSLocationAlwaysAndWhenInUseUsageDescription

A message that tells the user why the app is requesting access to the user’s location information at all times.

