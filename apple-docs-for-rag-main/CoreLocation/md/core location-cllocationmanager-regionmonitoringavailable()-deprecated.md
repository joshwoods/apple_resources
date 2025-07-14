

- Core Location
- CLLocationManager
-  regionMonitoringAvailable() Deprecated

Type Method

# regionMonitoringAvailable()

Returns a Boolean value indicating whether region monitoring is supported on the current device.

macOS 10.8–10.10DeprecatedvisionOS 1.0–1.0Deprecated

``` source
class func regionMonitoringAvailable() -> Bool
```

Deprecated

Use isMonitoringAvailable(for:) instead.

## Return Value

true if region monitoring is available; false if it is not.

## Discussion

Support for region monitoring may not be available on all devices and models. You should check the value of this property before attempting to set up any regions or initiate region monitoring.

Even if region monitoring support is present on a device, it may still be unavailable because the user disabled it for the current app or for all apps.

### Special Considerations

This class is deprecated in iOS 7 and later but is still supported in macOS.

## See Also

### Methods

func startMonitoring(for: CLRegion)

Starts monitoring the specified region.

Deprecated

func stopMonitoring(for: CLRegion)

Stops monitoring the specified region.

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

func disallowDeferredLocationUpdates()

Cancels the deferral of location updates for this app.

Deprecated

