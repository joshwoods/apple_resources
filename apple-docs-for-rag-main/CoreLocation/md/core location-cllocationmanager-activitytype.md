

- Core Location
- CLLocationManager
-  activityType 

Instance Property

# activityType

The type of activity the app expects the user to typically perform while in the app’s location session.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+watchOS 4.0+

``` source
var activityType: CLActivityType { get set }
```

## Mentioned in 

Getting the current location of a device

## Discussion

An app should use `activityType` to communicate to Core Location algorithms the type of activity the app’s users typically perform while using the app. The location manager uses the information in this property as a cue to determine when the system may pause location updates. Pausing updates gives the system the opportunity to save power in situations where the user’s location isn’t likely to be changing. For example, if the activity type is CLActivityType.automotiveNavigation and no location changes have occurred recently, the system might power down radios until the system detects movement again.

After a pause occurs, it’s your responsibility to restart location services again when you determine that they’re needed. For more information on ways to restart location services after a pause, see the discussion of the pausesLocationUpdatesAutomatically property.

The default value of this property is CLActivityType.other.

If your app allows the user to change the type activity they’re performing, for example in a navigation app that allows the user to switch between driving or walking modes, you should also update the `activityType` as well.

## See Also

### Running the standard location service

func startUpdatingLocation()

Starts the generation of updates that report the user’s current location.

func stopUpdatingLocation()

Stops the generation of location updates.

func requestLocation()

Requests the one-time delivery of the user’s current location.

var pausesLocationUpdatesAutomatically: Bool

A Boolean value that indicates whether the location-manager object may pause location updates.

var allowsBackgroundLocationUpdates: Bool

A Boolean value that indicates whether the app receives location updates when running in the background.

var showsBackgroundLocationIndicator: Bool

A Boolean value that indicates whether the status bar changes its appearance when an app uses location services in the background.

enum CLActivityType

Constants that indicate the type of activity associated with location updates.

