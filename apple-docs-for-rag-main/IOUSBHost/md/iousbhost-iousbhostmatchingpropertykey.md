

- IOUSBHost
-  IOUSBHostMatchingPropertyKey 

Structure

# IOUSBHostMatchingPropertyKey

Properties for implementing the matching service.

Mac Catalyst 14.0+macOS 10.15+

``` source
struct IOUSBHostMatchingPropertyKey
```

## Topics

### Device Properties

static let vendorID: IOUSBHostMatchingPropertyKey

The matching property for the device’s vendor ID.

static let productID: IOUSBHostMatchingPropertyKey

The matching property for the device’s product ID.

static let deviceReleaseNumber: IOUSBHostMatchingPropertyKey

The matching property for the device’s release number.

static let configurationValue: IOUSBHostMatchingPropertyKey

The matching property for the device’s current configuration value.

static let speed: IOUSBHostMatchingPropertyKey

The matching property for the device’s enumeration speed.

static let productIDArray: IOUSBHostMatchingPropertyKey

The matching property on a list of product IDs.

static let productIDMask: IOUSBHostMatchingPropertyKey

The matching property on a mask of product IDs.

### Interface Properties

static let interfaceNumber: IOUSBHostMatchingPropertyKey

The matching property for the device’s interface number.

static let interfaceClass: IOUSBHostMatchingPropertyKey

The matching property for the interface’s class ID.

static let interfaceSubClass: IOUSBHostMatchingPropertyKey

The matching property for the interface’s subclass ID.

static let interfaceProtocol: IOUSBHostMatchingPropertyKey

The matching property for the interface’s protocol.

### Protocol and Class Properties

static let deviceProtocol: IOUSBHostMatchingPropertyKey

The matching property for the device’s protocol.

static let deviceClass: IOUSBHostMatchingPropertyKey

The matching property for the device’s class.

static let deviceSubClass: IOUSBHostMatchingPropertyKey

The matching property for the device’s subclass.

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

struct IOUSBHostInterfacePropertyKey

Properties of a USB interface that describe its state.

struct IOUSBHostDevicePropertyKey

Properties of a USB device that describe its state.

typealias IOUSBHostPropertyKey

Properties that the USB host device and interface classes share.

