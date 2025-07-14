

- XCUIAutomation
- XCUIDevice
-  appearance 

Instance Property

# appearance

The interface style of the device.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+Xcode 16.3+

``` source
@MainActor
var appearance: XCUIDevice.Appearance { get set }
```

## Discussion

Use this property to get or set the interface appearance the system uses for applications running on the device. The example below captures the initial appearance value and sets the device to Dark Mode:

```
let previousAppearance = XCUIDevice.shared.appearance 
XCUIDevice.shared.appearance = .dark
```

Set the property once in your test fixture’s setup or intialization code to set an appearance for all the test methods in that fixture.

## See Also

### Interacting with the OS

var system: XCUISystem

An object that provides an interface to OS-specific properties and actions.

enum Appearance

Constants that indicate an interface style.

