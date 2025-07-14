

- Core Motion
- CMMotionActivity
-  unknown 

Instance Property

# unknown

A Boolean indicating whether the type of motion is unknown.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 15.0+watchOS 2.0+

``` source
var unknown: Bool { get }
```

## Discussion

This property is set to true when there is no way to estimate the current type of motion. For example, this property might be true if the device was turned on recently and not enough motion data had been gathered to determine the type of motion.

## See Also

### Getting the Type of Motion

var stationary: Bool

A Boolean indicating whether the device is stationary.

var walking: Bool

A Boolean indicating whether the device is on a walking person.

var running: Bool

A Boolean indicating whether the device is on a running person.

var automotive: Bool

A Boolean indicating whether the device is in an automobile.

var cycling: Bool

A Boolean indicating whether the device is in a bicycle.

