

- AppKit
- NSButtonCell
-  getPeriodicDelay(\_:interval:) 

Instance Method

# getPeriodicDelay(\_:interval:)

Returns by reference the delay and interval periods for a continuous button.

macOS

``` source
@MainActor
func getPeriodicDelay(
    _ delay: UnsafeMutablePointer,
    interval: UnsafeMutablePointer
)
```

## Parameters 

`delay`  

On return, the amount of time (in seconds) that the button will pause before starting to periodically send action messages to the target object. Default values are taken from the user’s defaults (60 seconds maximum); if the user hasn’t specified a default value, this defaults to 0.4 seconds.

`interval`  

On return, the amount of time (in seconds) between each action message. Default values are taken from the user’s defaults (60 seconds maximum); if the user hasn’t specified a default value, this defaults to 0.075 seconds.

## See Also

### Related Documentation

var isContinuous: Bool

A Boolean value indicating whether the cell sends its action message continuously during mouse tracking.

### Managing the Repeat Interval

func setPeriodicDelay(Float, interval: Float)

Sets the message delay and interval for the button.

