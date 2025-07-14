

- Core Motion
- CMStepCounter
-  isStepCountingAvailable() Deprecated

Type Method

# isStepCountingAvailable()

Returns a Boolean indicating whether step-counting support is available on the current device.

iOS 7.0–8.0DeprecatediPadOS 7.0–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedvisionOS 1.0–1.0Deprecated

``` source
class func isStepCountingAvailable() -> Bool
```

Deprecated

Use CMPedometer instead

## Return Value

true if step-counting support is available or false if it is not.

## Discussion

Step-counting support is not available on all iOS devices. Use this method to determine if support is available on the current device.

