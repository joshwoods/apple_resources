

- Core Location
- CLLocationManagerDelegate
-  locationManager(\_:monitoringDidFailFor:withError:) 

Instance Method

# locationManager(\_:monitoringDidFailFor:withError:)

Tells the delegate that a region monitoring error occurred.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.8+

``` source
optional func locationManager(
    _ manager: CLLocationManager,
    monitoringDidFailFor region: CLRegion?,
    withError error: any Error
)
```

## Parameters 

`manager`  

The location manager object reporting the event.

`region`  

The region for which the error occurred.

`error`  

An error object containing the error code that indicates why region monitoring failed.

## Discussion

If an error occurs while trying to monitor a given region, the location manager sends this message to its delegate. Region monitoring might fail because the region itself cannot be monitored or because there was a more general failure in configuring the region monitoring service.

Although implementation of this method is optional, it is recommended that you implement it if you use region monitoring in your application.

## See Also

### Related Documentation

func locationManager(CLLocationManager, didFailWithError: any Error)

Tells the delegate that the location manager was unable to retrieve a location value.

