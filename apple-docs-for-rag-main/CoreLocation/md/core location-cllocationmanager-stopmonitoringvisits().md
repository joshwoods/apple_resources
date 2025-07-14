

- Core Location
- CLLocationManager
-  stopMonitoringVisits() 

Instance Method

# stopMonitoringVisits()

Stops the delivery of visit-related events.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.15+

``` source
func stopMonitoringVisits()
```

## Discussion

Calling this method disables the delivery of visit-related events for your app. If a compatible iPad or iPhone app calls this method when running in visionOS, the method does nothing.

## See Also

### Running the visits location service

func startMonitoringVisits()

Starts the delivery of visit-related events.

