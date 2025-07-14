

- Core Location
- CLLocationManager
-  stopMonitoringLocationPushes() 

Instance Method

# stopMonitoringLocationPushes()

Stops monitoring for Apple Push Notification service (APNs) location pushes.

iOS 15.0+iPadOS 15.0+

``` source
func stopMonitoringLocationPushes()
```

## Discussion

Call this method to stop the device from monitoring for APNs location pushes. If a compatible iPad or iPhone app calls this method when running in visionOS, the method does nothing.

## See Also

### Monitoring location push notifications

func startMonitoringLocationPushes(completion: ((Data?, (any Error)?) -> Void)?)

Starts monitoring for the delivery of Apple Push Notification service (APNs) location pushes, and provides a device-specific token for sending pushes.

