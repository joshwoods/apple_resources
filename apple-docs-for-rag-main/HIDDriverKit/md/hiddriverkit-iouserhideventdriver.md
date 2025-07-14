

- HIDDriverKit
-  IOUserHIDEventDriver 

Class

# IOUserHIDEventDriver

A complete driver object that dispatches keyboard, digitizer, scrolling, and pointer events originating from a HID device.

DriverKitmacOS

``` source
class IOUserHIDEventDriver;
```

## Overview

An `IOUserHIDEventDriver` object is a fully functional driver that handles many common types of HID events. This driver parses incoming reports and uses the information to dispatch many types of events to the system. Apple provides this driver object as a default implementation for devices that conform to the HID specifications and don’t include any custom information that requires a special driver.

You can subclass `IOUserHIDEventDriver` and add support for other types of events. Alternatively, you can subclass IOUserHIDEventService and customize how your event service processes the report data.

### Specify the Driver’s Personality Information

When you subclass IOUserHIDEventDriver, update the `IOKitPersonalities` key of your driver extension’s `Info.plist` file with information to match your driver to appropriate hardware. For this class, always include the keys and values in the following table.

| Key | Discussion |
|----|----|
| `IOClass` | The value `AppleUserHIDEventService`. |
| `IOProviderClass` | The provider class information. For HID interfaces, specify IOHIDInterface. |
| `IOUserClass` | The name of your custom subclass. |
| CFBundleIdentifier | The bundle identifier of your driver. |

You may add other keys to assist with the matching process. For example, you might include the `VendorID`, `ProductID`, `PrimaryUsagePage`, and `PrimaryUsage` keys to match against specific USB devices and HID usage types. The USB specification defines which keys to include when matching your driver to a USB device. For information about the specific key combinations, see *Universal Serial Bus Common Class Specification* at https://www.usb.org.

## Topics

### Running the Driver

init

Handles the basic initialization of the event service.

Start

Starts the current event driver and associates it with the specified provider object.

free

Performs any final cleanup for the service.

### Parsing the Element Hierarchy

parseElements

Parses the specified array of elements.

parsePointerElement

Parses an element to see if it supports pointer usages.

parseDigitizerElement

Parses an element to see if it supports digitizer usages.

parseKeyboardElement

Parses an element to see if it contains keyboard-related information.

parseScrollElement

Parses an element to see if it supports scroll usages.

parseLEDElement

Parses an element to see if it supports LED usages.

### Handling New Data Reports

handleReport

Processes the information in a new device report and dispatches any relevant events in response.

handleKeyboardReport

Iterates through keyboard elements and dispatches them if the element value has been updated.

handleRelativePointerReport

Iterates through relative pointer elements and dispatches them if the element value has been updated.

handleAbsolutePointerReport

Iterates through absolute pointer elements and dispatches them if the element value has been updated.

handleScrollReport

Iterates through scroll elements and dispatches them if the element value has been updated.

handleDigitizerReport

Processes the digitizer elements and dispatches events for any updated values.

createEventForDigitizerCollection

Creates a HID event object that represents a digitizer collection.

### Configuring LED Lights

SetLED

Sets the state of an LED on the device.

### Configuring Private Properties

setAccelerationProperties

setSurfaceDimensions

setTipThreshold

### Instance Methods

SetProperties

calibrateCenteredPreferredStateElement

calibrateJustifiedPreferredStateElement

checkGameControllerElement

copyKeyboardEvent

getButtonStateFromElements

handleCopyMatchingEvent

handleGameControllerReport

handleProximityReport

parseElement

parseGameControllerElement

parseProximityElement

parseRemainingElement

parseRemainingElements

postProcessElements

postProcessElements_internal

processDigitizerElements

processGameControllerElements

setDigitizerProperties

setGameControllerProperties

setKeyboardProperties

setLEDProperties

setRelativeProperties

setScrollProperties

## Relationships

### Inherits From

- IOUserHIDEventService

## See Also

### Driver Interfaces

com.apple.developer.driverkit.family.hid.eventservice

A Boolean value that indicates whether the driver provides a HID-related event service to the system.

IOUserHIDEventService

A service that parses HID report data into elements that you can use to dispatch events.

IOHIDEventService

The base class for implementing a device or operating system service that dispatches events to the system.

