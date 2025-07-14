

- HIDDriverKit
-  IOUserUSBHostHIDDevice 

Class

# IOUserUSBHostHIDDevice

A provider object for USB devices that support HID interactions.

DriverKitmacOS

``` source
class IOUserUSBHostHIDDevice;
```

## Overview

An `IOUserUSBHostHIDDevice` object is a fully functional provider object that represents a USB-based HID device. Typically, you don’t create `IOUserUSBHostHIDDevice` objects directly. Instead, you specify that your driver relies on an `IOUserUSBHostHIDDevice` as its provider, and the system creates the interface object for you during the matching process.

When implementing a custom driver, use this provider object to manage the connection to the underlying device. Specifically, use it to get reports from the device and to manage the device’s configuration. For example, use the object to configure the USB device’s idle policy.

Subclass `IOUserUSBHostHIDDevice` only when you want to customize the interactions with the USB device. For example, you might use a custom subclass to initialize the USB device in a particular way or support a custom transport mechanism. You can also use a custom subclass to perform additional processing on the report data.

### Specify the Driver’s Personality Information

When you subclass `IOUserUSBHostHIDDevice`, update the `IOKitPersonalities` key of your driver extension’s `Info.plist` file with information to match your driver to appropriate hardware. For this class, always include the keys and values in the following table.

| Key | Discussion |
|----|----|
| `IOClass` | The value `AppleUserHIDDevice`. |
| `IOProviderClass` | The provider class information. For a USB-based HID device, specify IOUSBHostInterface. |
| `IOUserClass` | The name of your custom subclass. |
| CFBundleIdentifier | The bundle identifier of your driver. |

You may add other keys to assist with the matching process. For example, you might include the `VendorID`, `ProductID`, `PrimaryUsagePage`, and `PrimaryUsage` keys to match against specific USB devices and HID usage types. The USB specification defines which keys to include when matching your driver to a USB device. For information about the specific key combinations, see *Universal Serial Bus Common Class Specification* at https://www.usb.org.

## Topics

### Running the Service

init

Handles the basic initialization of the event service.

Start

Starts the current device service and associates it with the specified provider object.

handleStart

Performs any custom initialization associated with starting the device service.

Stop

Stops the device service associated with the specified provider.

free

Performs any final cleanup for the service.

### Getting the Device Description

newDeviceDescription

Creates and returns a new dictionary that describes the HID device.

### Managing Device Reports

newReportDescriptor

Returns the data in the HID device’s report descriptor.

getReport

Gets a report from the HID device.

getReport

Gets a report from the HID device.

setReport

Sends a report to the HID device.

initInputReport

Starts reading the input report from the device.

CompleteInputReport

Processes the results of an asynchronous request for an input report.

scheduleInputReportRetry

Retries a previous request for an input report.

cancelInputReportRetry

Cancels a retry attempt for an input report request.

TimerOccurred

Handles timeout-related actions when retrying input report requests.

### Configuring the Device

setProtocol

Sets the active protocol to use for communicating with the USB device.

setIdle

Sets the device’s idle time.

setIdlePolicy

Sets the amount of idle time that must pass before suspending the device.

setProperty

Updates the specified property on the corresponding kernel object.

reset

Resets the USB device.

USBIdlePolicyType

Constants that specify whether to apply the idle policy to an interface or pipe.

### Configuring Private Settings

initPipes

getHIDDescriptorInfo

CompleteZLP

copyStringAtIndex

### Instance Methods

CompleteOutputReport

CompleteOutputRequest

getAction

isBulkPipeSupported

returnAction

## Relationships

### Inherits From

- IOUserHIDDevice

## See Also

### Providers

com.apple.developer.driverkit.family.hid.device

A Boolean value that indicates whether the driver provides a HID-related service to the system.

IOHIDInterface

A provider object for a HID device’s interface.

IOUserHIDDevice

A provider object for devices that support interactions with users.

IOHIDDevice

An object containing the low-level behavior for all HID device providers.

