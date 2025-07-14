

- Core Location
- CLLocationManager
-  regionMonitoringEnabled() Deprecated

Type Method

# regionMonitoringEnabled()

Returns a Boolean value indicating whether region monitoring is currently enabled.

macOS 10.8–10.10DeprecatedvisionOS 1.0–1.0Deprecated

``` source
class func regionMonitoringEnabled() -> Bool
```

Deprecated

Use isMonitoringAvailable(for:) instead.

## Return Value

true if region monitoring is available and is currently enabled; false if it is unavailable or not enabled.

## Discussion

In iOS, the user can enable or disable location services (including region monitoring) using the controls in Settings \> Location Services.

You should check the return value of this method before starting region monitoring updates to determine whether the user currently allows location services to be used at all. If this method returns false and you start region monitoring updates anyway, the Core Location framework prompts the user to confirm asking whether location services should be reenabled.

This method does not check to see if region monitoring capabilities are actually supported by the device. Therefore, you should also check the return value of the regionMonitoringAvailable() class method before attempting to start region monitoring services.

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

func disallowDeferredLocationUpdates()

Cancels the deferral of location updates for this app.

Deprecated

