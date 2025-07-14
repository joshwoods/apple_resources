

- XCUIAutomation
- XCUIDevice
-  rotateDigitalCrown(delta:velocity:) 

Instance Method

# rotateDigitalCrown(delta:velocity:)

Simulates the user rotating the Digital Crown on an Apple Watch by the delta amount and speed you provide.

visionOSwatchOSXcode 16.3+

``` source
@MainActor
func rotateDigitalCrown(
    delta rotationalDelta: CGFloat,
    velocity: XCUIGestureVelocity
)
```

## Parameters 

`rotationalDelta`  

A float value that indicates the fraction of a full rotation of the Digital Crown.

`velocity`  

A value that represents how fast to rotate the Digital Crown, in rotations per second.

## Discussion

Provide a positive value for `rotationalDelta` to indicate scrolling upward or a negative value to indicate scrolling downward, regardless of the orientation of the watch. A `rotationalDelta` value of `1.0` indicates a full rotation of the Digital Crown. Specify a `velocity` in rotations per second; the system ignores the sign of the `velocity` you provide.

## See Also

### Interacting with buttons and the Digital Crown

func press(XCUIDevice.Button)

Simulates the user pressing a physical button.

func hasHardwareButton(XCUIDevice.Button) -> Bool

Determines whether the device supports the button type you provide.

enum Button

A physical button on an iOS device.

func rotateDigitalCrown(delta: CGFloat)

Simulates the user rotating the Digital Crown on an Apple Watch by the delta amount.

