

- XCUIAutomation
- XCUIDevice
-  XCUIDevice.Appearance 

Enumeration

# XCUIDevice.Appearance

Constants that indicate an interface style.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSXcode 16.3+

``` source
enum Appearance
```

## Topics

### Appearances

case unspecified

An unspecified interface style.

case light

The light interface style.

case dark

The dark interface style.

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

### Interacting with the OS

var system: XCUISystem

An object that provides an interface to OS-specific properties and actions.

var appearance: XCUIDevice.Appearance

The interface style of the device.

