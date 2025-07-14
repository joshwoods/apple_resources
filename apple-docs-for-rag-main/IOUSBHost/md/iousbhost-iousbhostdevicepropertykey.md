

- IOUSBHost
-  IOUSBHostDevicePropertyKey 

Structure

# IOUSBHostDevicePropertyKey

Properties of a USB device that describe its state.

Mac Catalyst 14.0+macOS 10.15+

``` source
struct IOUSBHostDevicePropertyKey
```

## Topics

### Properties

static let currentConfiguration: IOUSBHostDevicePropertyKey

The device’s current configuration value.

static let containerID: IOUSBHostDevicePropertyKey

The device’s container ID.

static let serialNumberString: IOUSBHostDevicePropertyKey

The device’s serial number as a string.

static let vendorString: IOUSBHostDevicePropertyKey

The device’s vendor name.

typealias IOUSBHostPropertyKey

Properties that the USB host device and interface classes share.

### Initializing the Properties

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

struct IOUSBHostInterfacePropertyKey

Properties of a USB interface that describe its state.

struct IOUSBHostMatchingPropertyKey

Properties for implementing the matching service.

typealias IOUSBHostPropertyKey

Properties that the USB host device and interface classes share.

