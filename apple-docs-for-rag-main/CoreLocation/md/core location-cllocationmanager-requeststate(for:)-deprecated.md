

- Core Location
- CLLocationManager
-  requestState(for:) Deprecated

Instance Method

# requestState(for:)

Retrieves the state of a region asynchronously.

iOS 5.0–18.4DeprecatediPadOS 5.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.8–11.0Deprecated

``` source
func requestState(for region: CLRegion)
```

Deprecated

Use CLMonitor to track and query the state for monitored constraints.

## Parameters 

`region`  

The region with the state you want to know. This object needs to be an instance of one of the standard region subclasses that Core Location provides, such as CLCircularRegion or CLBeaconRegion. You can’t use this method to determine the state of custom regions you define yourself.

## Discussion

This method performs the request asynchronously and delivers the results to the location manager’s delegate. You must implement the locationManager(_:didDetermineState:for:) method in the delegate to receive the results.

If the `region` parameter contains an unknown type of region object, this method does nothing. If a compatible iPad or iPhone app calls this method when running in visionOS, the method does nothing.

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

