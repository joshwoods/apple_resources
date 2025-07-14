

- XCUIAutomation
- XCUIDevice
-  press(\_:) 

Instance Method

# press(\_:)

Simulates the user pressing a physical button.

iOSiPadOSMac CatalysttvOSvisionOSwatchOSXcode 16.3+

``` source
@MainActor
func press(_ button: XCUIDevice.Button)
```

## Parameters 

`button`  

The button to press on the device.

## See Also

### Interacting with buttons and the Digital Crown

func hasHardwareButton(XCUIDevice.Button) -> Bool

Determines whether the device supports the button type you provide.

enum Button

A physical button on an iOS device.

func rotateDigitalCrown(delta: CGFloat)

Simulates the user rotating the Digital Crown on an Apple Watch by the delta amount.

func rotateDigitalCrown(delta: CGFloat, velocity: XCUIGestureVelocity)

Simulates the user rotating the Digital Crown on an Apple Watch by the delta amount and speed you provide.

