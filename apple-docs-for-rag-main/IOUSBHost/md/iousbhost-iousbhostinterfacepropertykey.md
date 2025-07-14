

- IOUSBHost
-  IOUSBHostInterfacePropertyKey 

Structure

# IOUSBHostInterfacePropertyKey

Properties of a USB interface that describe its state.

Mac Catalyst 14.0+macOS 10.15+

``` source
struct IOUSBHostInterfacePropertyKey
```

## Topics

### Properties

static let alternateSetting: IOUSBHostInterfacePropertyKey

The USB interface’s current alternative setting value.

### Initializing the Structure

init(rawValue: String)

Creates the structure.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### IOServicePlane Properties

struct IOUSBHostDevicePropertyKey

Properties of a USB device that describe its state.

struct IOUSBHostMatchingPropertyKey

Properties for implementing the matching service.

typealias IOUSBHostPropertyKey

Properties that the USB host device and interface classes share.

