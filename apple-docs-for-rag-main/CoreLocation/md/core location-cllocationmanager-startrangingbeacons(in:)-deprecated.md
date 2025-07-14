

- Core Location
- CLLocationManager
-  startRangingBeacons(in:) Deprecated

Instance Method

# startRangingBeacons(in:)

Starts the delivery of notifications for the specified beacon region.

iOS 7.0–13.0DeprecatediPadOS 7.0–13.0DeprecatedMac Catalyst 14.0–14.0DeprecatedmacOS 11.0–11.0Deprecated

``` source
func startRangingBeacons(in region: CLBeaconRegion)
```

Deprecated

Use startRangingBeacons(satisfying:) instead.

## Parameters 

`region`  

The region object that defines the identifying information for the targeted beacons. The number of beacons represented by this region object depends on which identifier values you use to initialize it. Beacons must match all of the identifiers you specify. This method copies the region information it needs from the object you provide.

## Mentioned in 

Determining the proximity to an iBeacon device

## Discussion

Once registered, the location manager reports any encountered beacons to its delegate by calling the locationManager(_:didRangeBeacons:in:) method. If there is an error registering the specified beacon region, the location manager calls its delegate’s locationManager(_:rangingBeaconsDidFailFor:withError:) method and provides the appropriate error information.

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

