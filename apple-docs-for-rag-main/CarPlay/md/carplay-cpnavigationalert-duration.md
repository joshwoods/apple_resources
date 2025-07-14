

- CarPlay
- CPNavigationAlert
-  duration 

Instance Property

# duration

The amount of time, in seconds, that the alert is visible.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
var duration: TimeInterval { get }
```

## Discussion

Set `duration` to zero to display the alert until dismissed by the user. When `duration` is not zero, CPNavigationAlertMinimumDuration determines the minimum amount of time the alert is visible.

## See Also

### Getting the Alert Duration

let CPNavigationAlertMinimumDuration: TimeInterval

A constant that defines the minimum amount of time that an alert is visible.

