

- Core Location
- CLLocationManager
-  startMonitoring(for:) Deprecated

Instance Method

# startMonitoring(for:)

Starts monitoring the specified region.

iOS 5.0–18.4DeprecatediPadOS 5.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.8–11.0Deprecated

``` source
func startMonitoring(for region: CLRegion)
```

Deprecated

Use addConditionForMonitoring:identifier: instead.

## Parameters 

`region`  

The region object that defines the boundary to monitor. This parameter must not be `nil`.

## Mentioned in 

Monitoring the user’s proximity to geographic regions

Determining the proximity to an iBeacon device

## Discussion

You must call this method once for each region you want to monitor. If an existing region with the same identifier is already being monitored by the app, the old region is replaced by the new one. The regions you add using this method are shared by all location manager objects in your app and stored in the monitoredRegions property.

Region events are delivered to the locationManager(_:didEnterRegion:) and locationManager(_:didExitRegion:) methods of your delegate. If there is an error, the location manager calls the locationManager(_:monitoringDidFailFor:withError:) method of your delegate instead.

An app can register up to 20 regions at a time. In order to report region changes in a timely manner, the region monitoring service requires network connectivity.

In iOS 6, regions with a radius between 1 and 400 meters work better on iPhone 4S or later devices. (In iOS 5, regions with a radius between 1 and 150 meters work better on iPhone 4S and later devices.) On these devices, an app can expect to receive the appropriate region entered or region exited notification within 3 to 5 minutes on average, if not sooner.

If a compatible iPad or iPhone app calls this method when running in visionOS, the method does nothing.

## See Also

### Methods

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

func disallowDeferredLocationUpdates()

Cancels the deferral of location updates for this app.

Deprecated

