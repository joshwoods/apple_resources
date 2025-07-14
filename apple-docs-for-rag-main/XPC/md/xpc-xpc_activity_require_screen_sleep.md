

- XPC
-  XPC_ACTIVITY_REQUIRE_SCREEN_SLEEP 

Global Variable

# XPC_ACTIVITY_REQUIRE_SCREEN_SLEEP

A Boolean value that indicates whether the activity performs only while the primary screen is in sleep mode.

macOS 10.9+

``` source
let XPC_ACTIVITY_REQUIRE_SCREEN_SLEEP: UnsafePointer
```

## Discussion

Defaults to `false`.

## See Also

### Power consumption

let XPC_ACTIVITY_ALLOW_BATTERY: UnsafePointer&lt;CChar>

A Boolean value that indicates whether to allow the activity to run while the computer is on battery power.

let XPC_ACTIVITY_PREVENT_DEVICE_SLEEP: UnsafePointer&lt;CChar>

A Boolean that indicates whether the activity prevents the system from sleeping while on battery power.

