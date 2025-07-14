

- Core Location
- CLLocationManager
-  disallowDeferredLocationUpdates() Deprecated

Instance Method

# disallowDeferredLocationUpdates()

Cancels the deferral of location updates for this app.

iOS 6.0–13.0DeprecatediPadOS 6.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.15–10.15Deprecated

``` source
func disallowDeferredLocationUpdates()
```

Deprecated

You can remove calls to this method

## Discussion

Call this method if you previously deferred location event delivery using the allowDeferredLocationUpdates(untilTraveled:timeout:) method and now want to resume the delivery of events at normal intervals.

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

class func deferredLocationUpdatesAvailable() -> Bool

Returns a Boolean value indicating whether the device supports deferred location updates.

Deprecated

func allowDeferredLocationUpdates(untilTraveled: CLLocationDistance, timeout: TimeInterval)

Asks the location manager to defer the delivery of location updates until the specified criteria are met.

Deprecated

