

- Core Location
- CLLocationManager
-  deferredLocationUpdatesAvailable() Deprecated

Type Method

# deferredLocationUpdatesAvailable()

Returns a Boolean value indicating whether the device supports deferred location updates.

iOS 6.0–13.0DeprecatediPadOS 6.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.9–10.15Deprecated

``` source
class func deferredLocationUpdatesAvailable() -> Bool
```

Deprecated

You can remove calls to this method

## Return Value

true if the device supports deferred location updates or false if it does not.

## Discussion

Deferred location updates are a way for the location manager to avoid frequently waking up a background app to deliver location changes. Normally, when an app wants location updates in the background, the app must be woken up whenever a new event arrives. Waking up the app consumes power, which in some situations might be wasted if the app cannot do anything with the location information other than log it and go back to sleep anyway. Deferring location updates gives you the ability to wait until a time when your app can do something useful with the data and then process the updates all at once.

Deferred location updates require the presence of GPS hardware and may not be supported on all iOS devices.

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

class func authorizationStatus() -> CLAuthorizationStatus

Returns the app’s authorization status for using location services.

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

func allowDeferredLocationUpdates(untilTraveled: CLLocationDistance, timeout: TimeInterval)

Asks the location manager to defer the delivery of location updates until the specified criteria are met.

Deprecated

func disallowDeferredLocationUpdates()

Cancels the deferral of location updates for this app.

Deprecated

