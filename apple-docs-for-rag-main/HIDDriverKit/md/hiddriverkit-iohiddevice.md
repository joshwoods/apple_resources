

- HIDDriverKit
-  IOHIDDevice 

Class

# IOHIDDevice

An object containing the low-level behavior for all HID device providers.

DriverKitmacOS

``` source
class IOHIDDevice;
```

## Overview

`IOHIDDevice` is the abstract base class for provider objects that represent a human interface device. This class defines the basic interface that subclasses use to manage reports. Don’t create instances of this class directly. Instead, subclass IOUserHIDDevice or IOUserUSBHostHIDDevice to define the behavior of your custom device provider.

## Topics

### Processing Device Reports

handleReport

Handles an asynchronous report received from the HID device.

getReport

Gets a report from the HID device.

setReport

Sends a report to the HID device.

CompleteReport

Completes all async requests made when getting or setting a report.

Report Options

The enumerated report options.

### Setting Device Properties

setProperty

Updates the specified property on the corresponding kernel object.

## Relationships

### Inherits From

- IOService

### Inherited By

- IOUserHIDDevice

## See Also

### Providers

com.apple.developer.driverkit.family.hid.device

A Boolean value that indicates whether the driver provides a HID-related service to the system.

IOHIDInterface

A provider object for a HID device’s interface.

IOUserUSBHostHIDDevice

A provider object for USB devices that support HID interactions.

IOUserHIDDevice

A provider object for devices that support interactions with users.

