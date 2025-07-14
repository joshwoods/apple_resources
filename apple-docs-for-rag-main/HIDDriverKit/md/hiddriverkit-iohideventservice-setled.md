

- HIDDriverKit
- IOHIDEventService
-  SetLED 

Instance Method

# SetLED

Configures the on/off state for an LED on the device.

DriverKit 19.0+macOS

``` source
void SetLED(uint32_t usage, bool on);
```

## Parameters 

`usage`  

The usage value that matches the LED you want to set. For a list of possible values, see LEDs.

`on`  

A Boolean value that indicates whether to turn the light on or off. Specify `true` to turn the light on or `false` to turn it off.

