

- HIDDriverKit
- IOUserHIDEventDriver
-  SetLED 

Instance Method

# SetLED

Sets the state of an LED on the device.

DriverKit 19.0+macOS

``` source
void SetLED(uint32_t usage, bool on);
```

## Parameters 

`usage`  

The LED to set. Specify a value from the LED usage tables in LEDs.

`on`  

A Boolean value that indicates whether to turn the LED on or off. Specify `true` to turn the LED on.

