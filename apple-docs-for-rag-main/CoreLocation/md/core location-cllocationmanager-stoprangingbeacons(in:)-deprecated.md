

- Core Location
- CLLocationManager
-  stopRangingBeacons(in:) Deprecated

Instance Method

# stopRangingBeacons(in:)

Stops the delivery of notifications for the specified beacon region.

iOS 7.0–13.0DeprecatediPadOS 7.0–13.0DeprecatedMac Catalyst 14.0–14.0DeprecatedmacOS 11.0–11.0Deprecated

``` source
func stopRangingBeacons(in region: CLBeaconRegion)
```

Deprecated

Use stopRangingBeacons(satisfying:) instead.

## Parameters 

`region`  

The region that identifies the beacons. The object you specify need not be the exact same object that you registered but the beacon attributes should be the same.

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

class func deferredLocationUpdatesAvailable() -> Bool

Returns a Boolean value indicating whether the device supports deferred location updates.

Deprecated

func allowDeferredLocationUpdates(untilTraveled: CLLocationDistance, timeout: TimeInterval)

Asks the location manager to defer the delivery of location updates until the specified criteria are met.

Deprecated

func disallowDeferredLocationUpdates()

Cancels the deferral of location updates for this app.

Deprecated

