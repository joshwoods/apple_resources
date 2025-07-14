

- Core Location
- CLLocationManager
-  requestTemporaryFullAccuracyAuthorization(withPurposeKey:completion:) 

Instance Method

# requestTemporaryFullAccuracyAuthorization(withPurposeKey:completion:)

Requests permission to temporarily use location services with full accuracy and reports the results to the provided completion handler.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
func requestTemporaryFullAccuracyAuthorization(
    withPurposeKey purposeKey: String,
    completion: (((any Error)?) -> Void)? = nil
)
```

``` source
func requestTemporaryFullAccuracyAuthorization(withPurposeKey purposeKey: String) async throws
```

## Parameters 

`purposeKey`  

A key in the NSLocationTemporaryUsageDescriptionDictionary dictionary of the app’s `Info.plist` file. The value for this key is an app-provided string that describes the reason for accessing location data with full accuracy. To localize a usage description, add an entry to your `InfoPlist.strings` file with the same key you provide for this parameter.

`completion`  

A closure to execute after authorization status changes. This closure takes a single `error` parameter, which is `nil` if the prompt was displayed to the user, or an error object describing why the prompt couldn’t be displayed.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func requestTemporaryFullAccuracyAuthorization(withPurposeKey purposeKey: String) async throws
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

After the user gives permission for your app to use location data with full accuracy, your app can access that data in the foreground or in the background, until its permission automatically expires. Expiration is postponed while your app is actively in use. For example, expiration is postponed while your app in the foreground, and while a Continuous Background Location session is active with the background location indicator enabled. This approach to expiration allows apps to provide experiences that require full accuracy, such as fitness and navigation apps, even if the user doesn’t grant persistent access for full accuracy.

The completion closure is guaranteed to be called after the request is completed, which includes the user granting access, the user declining, or an error that prevented displaying the prompt. The closure is always called in the same threading context as CLLocationManagerDelegate methods. If the prompt was successfully displayed to the user, the callback’s `error` parameter is `nil`.

The request always fails with a CLError.Code.promptDeclined error in the following cases:

- The `Info.plist` file doesn’t have an entry for the given `purposeKey` value.

- The app is already authorized for full accuracy.

- The app is in the background.

If the closure is called with an error, log the error for debugging purposes, and retry the request again the next time the user performs the action that caused you to request precise location information.

## See Also

### Requesting authorization for location services

func requestWhenInUseAuthorization()

Requests the user’s permission to use location services while the app is in use.

func requestAlwaysAuthorization()

Requests the user’s permission to use location services regardless of whether the app is in use.

func requestTemporaryFullAccuracyAuthorization(withPurposeKey: String)

Requests permission to temporarily use location services with full accuracy.

var authorizationStatus: CLAuthorizationStatus

The current authorization status for the app.

enum CLAuthorizationStatus

Constants that indicate the app’s authorization to use location services.

NSLocationDefaultAccuracyReduced

A Boolean value that indicates whether the app requests reduced location accuracy by default.

NSLocationAlwaysAndWhenInUseUsageDescription

A message that tells the user why the app is requesting access to the user’s location information at all times.

