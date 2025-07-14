

- Core Location
- CLLocationManager
-  startMonitoring(for:desiredAccuracy:) Deprecated

Instance Method

# startMonitoring(for:desiredAccuracy:)

Starts monitoring the specified region for boundary crossings.

macOS 10.15–10.15Deprecated

``` source
func startMonitoring(
    for region: CLRegion,
    desiredAccuracy accuracy: CLLocationAccuracy
)
```

Deprecated

Use startMonitoring(for:) instead.

## Parameters 

`region`  

The region object that defines the boundary to monitor. This parameter must not be `nil`.

`accuracy`  

The distance past the border (measured in meters) at which to generate notifications. You can use this value to prevent the delivery of multiple notifications when the user is close to the border’s edge.

## Discussion

You must call this method separately for each region you want to monitor. If an existing region with the same identifier is already being monitored by the app, the old region is replaced by the new one. The regions you add using this method are shared by all location manager objects in your app and stored in the monitoredRegions property.

If you begin monitoring a region and your app is subsequently terminated, the system automatically relaunches it into the background if the region boundary is crossed. In such a case, the options dictionary passed to the application(_:didFinishLaunchingWithOptions:) method of your app delegate contains the key location to indicate that your app was launched because of a location-related event. In addition, creating a new location manager and assigning a delegate results in the delivery of the corresponding region messages. The newly created location manager’s location property also contains the current location even if location services are not enabled.

Region events are delivered to the locationManager(_:didEnterRegion:) and locationManager(_:didExitRegion:) methods of your delegate. If there is an error, the location manager calls the locationManager(_:monitoringDidFailFor:withError:) method of your delegate instead.

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

