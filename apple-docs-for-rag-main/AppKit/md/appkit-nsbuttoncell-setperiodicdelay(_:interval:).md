

- AppKit
- NSButtonCell
-  setPeriodicDelay(\_:interval:) 

Instance Method

# setPeriodicDelay(\_:interval:)

Sets the message delay and interval for the button.

macOS

``` source
@MainActor
func setPeriodicDelay(
    _ delay: Float,
    interval: Float
)
```

## Parameters 

`delay`  

The amount of time (in seconds) that a continuous button will pause before starting to periodically send action messages to the target object.

The maximum value is 60.0 seconds; if a larger value is supplied, it’s ignored, and 60.0 seconds is used.

`interval`  

The amount of time (in seconds) between each action message.

The maximum value is 60.0 seconds; if a larger value is supplied, it’s ignored, and 60.0 seconds is used.

## Discussion

These values are used if the button is configured (by a isContinuous message) to continuously send the action message to the target object while tracking the mouse.

## See Also

### Related Documentation

var isContinuous: Bool

A Boolean value indicating whether the cell sends its action message continuously during mouse tracking.

### Managing the Repeat Interval

func getPeriodicDelay(UnsafeMutablePointer&lt;Float>, interval: UnsafeMutablePointer&lt;Float>)

Returns by reference the delay and interval periods for a continuous button.

