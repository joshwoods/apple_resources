

- XPC
-  XPC_ACTIVITY_PREVENT_DEVICE_SLEEP 

Global Variable

# XPC_ACTIVITY_PREVENT_DEVICE_SLEEP

A Boolean that indicates whether the activity prevents the system from sleeping while on battery power.

macOS 12.0+

``` source
let XPC_ACTIVITY_PREVENT_DEVICE_SLEEP: UnsafePointer
```

## Discussion

When set to `true`, the activity scheduler takes the necessary power assertions to keep the device awake, excluding the screen. Only set this property for activities that perform critical system functions, and that system sleep can’t interrupt. Note that setting this property can affect battery life.

## See Also

### Power consumption

let XPC_ACTIVITY_ALLOW_BATTERY: UnsafePointer&lt;CChar>

A Boolean value that indicates whether to allow the activity to run while the computer is on battery power.

let XPC_ACTIVITY_REQUIRE_SCREEN_SLEEP: UnsafePointer&lt;CChar>

A Boolean value that indicates whether the activity performs only while the primary screen is in sleep mode.

