

- Core Location
- CLLocationManagerDelegate
-  locationManagerDidResumeLocationUpdates(\_:) 

Instance Method

# locationManagerDidResumeLocationUpdates(\_:)

Tells the delegate that the delivery of location updates has resumed.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
optional func locationManagerDidResumeLocationUpdates(_ manager: CLLocationManager)
```

## Parameters 

`manager`  

The location manager that resumed the delivery of events.

## Discussion

When you restart location services after an automatic pause, Core Location calls this method to notify your app that services have resumed. You are responsible for restarting location services in your app. Core Location does not resume updates automatically after it pauses them. For tips on how to restart location services when a pause occurs, see the discussion of the locationManagerDidPauseLocationUpdates(_:) method.

## See Also

### Pausing location updates

func locationManagerDidPauseLocationUpdates(CLLocationManager)

Tells the delegate that location updates were paused.

