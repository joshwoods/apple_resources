

- Core Location
- CLLocationManagerDelegate
-  locationManager(\_:didVisit:) 

Instance Method

# locationManager(\_:didVisit:)

Tells the delegate that a new visit-related event was received.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.15+

``` source
optional func locationManager(
    _ manager: CLLocationManager,
    didVisit visit: CLVisit
)
```

## Parameters 

`manager`  

The location manager object reporting the event.

`visit`  

The visit object that contains the information about the event.

## Discussion

The location manager calls this method whenever it has new visit event to report to your app.

