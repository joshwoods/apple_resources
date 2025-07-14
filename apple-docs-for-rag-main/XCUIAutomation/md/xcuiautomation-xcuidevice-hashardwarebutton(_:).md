

- XCUIAutomation
- XCUIDevice
-  hasHardwareButton(\_:) 

Instance Method

# hasHardwareButton(\_:)

Determines whether the device supports the button type you provide.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+Xcode 16.3+

``` source
@MainActor
func hasHardwareButton(_ button: XCUIDevice.Button) -> Bool
```

## Parameters 

`button`  

The type of physical button on an iOS device to check for.

## Return Value

`True` if the device has this type of button, otherwise `False`.

## Discussion

Use this method to check if the device supports the particular button type you provide.

## See Also

### Interacting with buttons and the Digital Crown

func press(XCUIDevice.Button)

Simulates the user pressing a physical button.

enum Button

A physical button on an iOS device.

func rotateDigitalCrown(delta: CGFloat)

Simulates the user rotating the Digital Crown on an Apple Watch by the delta amount.

func rotateDigitalCrown(delta: CGFloat, velocity: XCUIGestureVelocity)

Simulates the user rotating the Digital Crown on an Apple Watch by the delta amount and speed you provide.

