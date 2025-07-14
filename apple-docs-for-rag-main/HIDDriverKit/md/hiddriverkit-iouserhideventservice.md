

- HIDDriverKit
-  IOUserHIDEventService 

Class

# IOUserHIDEventService

A service that parses HID report data into elements that you can use to dispatch events.

DriverKitmacOS

``` source
class IOUserHIDEventService;
```

## Overview

Subclass `IOUserHIDEventService` when you want to process incoming data from a HID device before dispatching it to the system. An event service collects the report from a device, parses it into individual data elements, and dispatches events based on the information in those elements. Create a custom event service when you need to synthesize custom event data, or when you need to process the existing data before dispatching the corresponding events.

To implement a custom event service, override the handleReport method and use it to iterate over the report contents and dispatch any relevant events. To get the report data, call the getElements method each time a new report arrives. (Also call that method in your service’s Start method to create the elements initially.) The method returns a set of IOHIDElement objects that contain a parsed version of the report data. Each time you call the method, the system updates the elements to incorporate the data from the latest report.

### Specify the Driver’s Personality Information

When you subclass `IOUserHIDEventService`, update the `IOKitPersonalities` key of your driver extension’s `Info.plist` file with information to match your driver to appropriate hardware. For this class, always include the keys and values in the following table.

| Key | Discussion |
|----|----|
| `IOClass` | The value `AppleUserHIDEventService`. |
| `IOProviderClass` | The provider class information. For HID interfaces, specify IOHIDInterface. |
| `IOUserClass` | The name of your custom subclass. |
| CFBundleIdentifier | The bundle identifier of your driver. |

You may add other keys to assist with the matching process. For example, you might include the `VendorID`, `ProductID`, `PrimaryUsagePage`, and `PrimaryUsage` keys to match against specific USB devices and HID usage types. The USB specification defines which keys to include when matching your driver to a USB device. For information about the specific key combinations, see *Universal Serial Bus Common Class Specification* at https://www.usb.org.

## Topics

### Running the Service

init

Handles the basic initialization of the event service.

Start

Starts the current event service and associates it with the specified provider object.

handleStart

Performs additional initialization during the startup of the event service.

Stop

Stops the event service associated with the specified provider.

free

Performs any final cleanup for the service.

### Responding to Input Reports

getElements

Returns an array of elements that contain the parsed data from the HID device’s report.

handleReport

Converts an incoming device report into dispatchable events.

ReportAvailable

Notifies the event service that an updated report is available from the HID device.

### Dispatching Events to the System

dispatchDigitizerStylusEvent

Dispatches a digitizer stylus event to the system.

dispatchDigitizerTouchEvent

Dispatches a digitizer touch event to the system.

### Checking the Supported Usage

conformsTo

Returns a Boolean value that indicates whether the service conforms to the specified HID usage and page information.

### Performing Private Tasks

createReportPool

dispatchEvent

Dispatches a HID event to the system.

### Instance Methods

SetLEDState

SetProperties

dispatchExtendedGameControllerEvent

dispatchExtendedGameControllerEventWithOptionalButtons

dispatchStandardGameControllerEvent

processReport

## Relationships

### Inherits From

- IOHIDEventService

### Inherited By

- IOUserHIDEventDriver

## See Also

### Driver Interfaces

com.apple.developer.driverkit.family.hid.eventservice

A Boolean value that indicates whether the driver provides a HID-related event service to the system.

IOUserHIDEventDriver

A complete driver object that dispatches keyboard, digitizer, scrolling, and pointer events originating from a HID device.

IOHIDEventService

The base class for implementing a device or operating system service that dispatches events to the system.

