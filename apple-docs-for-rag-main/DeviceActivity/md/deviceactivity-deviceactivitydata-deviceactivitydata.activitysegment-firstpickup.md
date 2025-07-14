

- DeviceActivity
- DeviceActivityData
- DeviceActivityData.ActivitySegment
-  firstPickup 

Instance Property

# firstPickup

The first time the user picked up the device during the activity segment.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
var firstPickup: Date?
```

## Discussion

This value may be `nil` if the device was never picked up during dateInterval.

