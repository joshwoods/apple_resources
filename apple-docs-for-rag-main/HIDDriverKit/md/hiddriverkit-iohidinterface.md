

- HIDDriverKit
-  IOHIDInterface 

Class

# IOHIDInterface

A provider object for a HID device’s interface.

DriverKitmacOS

``` source
class IOHIDInterface;
```

## Overview

An `IOHIDInterface` object represents a specific interface of the HID device. Typically, you don’t create `IOHIDInterface` objects directly. Instead, you specify that your driver relies on an `IOHIDInterface` as its provider, and the system creates the interface object for you during the matching process.

To use a HID interface object directly, call Open to create a new session between the interface and your custom driver. When calling that method, you specify an OSAction object to execute each time a new report is ready to process. When a new report arrives, the `IOHIDInterface` object parses the device’s report data, puts the data into a set of IOHIDElement objects, and notifies your action object. Use your action object’s ReportAvailable method to parse the element objects and dispatch events.

## Topics

### Running the Interface

init

Handles the basic initialization of the interface.

free

### Managing the Session

Open

Opens a session to the device and begins the delivery of input reports.

Close

Closes the interface and stops the delivery of input reports.

### Getting and Setting Input Reports

ReportAvailable

Notifies the interface that an updated report is available from the HID device.

AddReportToPool

Adds a memory descriptor to the report pool.

processReport

Parses the contents of the specified report and updates the interface’s elements.

GetReport

Retrieves a new input report from the HID device.

SetReport

Sends a report to the HID device.

### Accessing the Elements of a Report

getElements

Returns the array of elements that the interface uses to store parsed report data.

commitElements

Gets or sets the contents of the interface’s stored elements.

## Relationships

### Inherits From

- IOService

## See Also

### Providers

com.apple.developer.driverkit.family.hid.device

A Boolean value that indicates whether the driver provides a HID-related service to the system.

IOUserUSBHostHIDDevice

A provider object for USB devices that support HID interactions.

IOUserHIDDevice

A provider object for devices that support interactions with users.

IOHIDDevice

An object containing the low-level behavior for all HID device providers.

