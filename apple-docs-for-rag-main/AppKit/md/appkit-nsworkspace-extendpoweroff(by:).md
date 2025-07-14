

- AppKit
- NSWorkspace
-  extendPowerOff(by:) 

Instance Method

# extendPowerOff(by:)

Requests the system wait for the specified amount of time before turning off the power or logging out the user.

macOS

``` source
func extendPowerOff(by requested: Int) -> Int
```

## Parameters 

`requested`  

The number of milliseconds to wait before turning off the power or logging off the user.

## Return Value

The number of milliseconds granted by the system. This method currently returns `0`.

## Discussion

This method currently does nothing. Do not call it.

