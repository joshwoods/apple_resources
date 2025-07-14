

- Core Location
- CLLocationManager
-  stopMonitoringSignificantLocationChanges() 

Instance Method

# stopMonitoringSignificantLocationChanges()

Stops the delivery of location events based on significant location changes.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+

``` source
func stopMonitoringSignificantLocationChanges()
```

## Discussion

Use this method to stop the delivery of location events that was started using the startMonitoringSignificantLocationChanges() method. If a compatible iPad or iPhone app calls this method when running in visionOS, the method does nothing.

## See Also

### Running the significant change location service

func startMonitoringSignificantLocationChanges()

Starts the generation of updates based on significant location changes.

