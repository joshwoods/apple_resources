

- DeviceActivity
- DeviceActivityData
- DeviceActivityData.ActivitySegment
-  longestActivity 

Instance Property

# longestActivity

The date interval of the user’s longest activity session during the activity segment.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
var longestActivity: DateInterval?
```

## Discussion

This value may be `nil` if the user was not active on this device during dateInterval.

