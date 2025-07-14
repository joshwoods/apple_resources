

- Core Location
- CLLocationManager
-  authorizationStatus() Deprecated

Type Method

# authorizationStatus()

Returns the app’s authorization status for using location services.

iOS 4.2–14.0DeprecatediPadOS 4.2–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedmacOS 10.7–11.0DeprecatedtvOS 9.0–14.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 1.0–7.0Deprecated

``` source
class func authorizationStatus() -> CLAuthorizationStatus
```

Deprecated

Use the authorizationStatus instance property with locationManagerDidChangeAuthorization(_:) instead.

## Return Value

A value indicating whether the app is authorized to use location services.

## Discussion

The system is guaranteed to call the delegate method with the app’s initial authorization state and all authorization status changes.

The system manages the authorization status of a given app according to several factors. Users must authorize the app to use location services explicitly, and location services must be enabled in Settings \> Privacy. See Choosing the Location Services Authorization to Request for more information.

## See Also

### Methods

func startMonitoring(for: CLRegion)

Starts monitoring the specified region.

Deprecated

func stopMonitoring(for: CLRegion)

Stops monitoring the specified region.

Deprecated

class func regionMonitoringAvailable() -> Bool

Returns a Boolean value indicating whether region monitoring is supported on the current device.

Deprecated

class func regionMonitoringEnabled() -> Bool

Returns a Boolean value indicating whether region monitoring is currently enabled.

Deprecated

func startMonitoring(for: CLRegion, desiredAccuracy: CLLocationAccuracy)

Starts monitoring the specified region for boundary crossings.

Deprecated

func requestState(for: CLRegion)

Retrieves the state of a region asynchronously.

Deprecated

func startRangingBeacons(in: CLBeaconRegion)

Starts the delivery of notifications for the specified beacon region.

Deprecated

func stopRangingBeacons(in: CLBeaconRegion)

Stops the delivery of notifications for the specified beacon region.

Deprecated

class func deferredLocationUpdatesAvailable() -> Bool

Returns a Boolean value indicating whether the device supports deferred location updates.

Deprecated

func allowDeferredLocationUpdates(untilTraveled: CLLocationDistance, timeout: TimeInterval)

Asks the location manager to defer the delivery of location updates until the specified criteria are met.

Deprecated

func disallowDeferredLocationUpdates()

Cancels the deferral of location updates for this app.

Deprecated

