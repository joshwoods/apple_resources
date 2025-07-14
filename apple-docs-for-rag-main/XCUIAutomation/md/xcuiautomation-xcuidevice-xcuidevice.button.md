

- XCUIAutomation
- XCUIDevice
-  XCUIDevice.Button 

Enumeration

# XCUIDevice.Button

A physical button on an iOS device.

iOSiPadOSMac CatalysttvOSvisionOSwatchOSXcode 16.3+

``` source
enum Button
```

## Overview

The XCUIDevice.Button.volumeUp and XCUIDevice.Button.volumeDown buttons aren’t available in Simulator. Use `targetEnvironment(simulator)` in Swift, or `TARGET_OS_SIMULATOR` in Objective-C, to check that your test isn’t running in Simulator before calling these APIs.

## Topics

### Device buttons

case home

The device’s home button.

case volumeUp

The device’s volume up button.

case volumeDown

The device’s volume down button.

case action

The device’s action button.

case camera

The device’s camera button.

### Initializers

init?(rawValue: Int)

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Interacting with buttons and the Digital Crown

func press(XCUIDevice.Button)

Simulates the user pressing a physical button.

func hasHardwareButton(XCUIDevice.Button) -> Bool

Determines whether the device supports the button type you provide.

func rotateDigitalCrown(delta: CGFloat)

Simulates the user rotating the Digital Crown on an Apple Watch by the delta amount.

func rotateDigitalCrown(delta: CGFloat, velocity: XCUIGestureVelocity)

Simulates the user rotating the Digital Crown on an Apple Watch by the delta amount and speed you provide.

