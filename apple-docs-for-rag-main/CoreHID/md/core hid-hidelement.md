

- Core HID
-  HIDElement 

Structure

# HIDElement

A representation of an item from a report descriptor for a HID device.

macOS 15.0+

``` source
struct HIDElement
```

## Mentioned in 

Communicating with human interface devices

## Overview

A HIDElement is an abstraction for the data in a HID report, and represents one item of data that could be sent or received in a report for a specific device. For example, for a mouse with a report descriptor that declares a report with 1 byte of data for each an X and a Y coordinate, there would be an element for the data associated with the X coordinate. If this element was monitored by a HIDDeviceClient, when an input report was received with an update to the X coordinate, a notification with the updated data would be sent to HIDDeviceClient.Notification.elementUpdates(values:).

Elements are only received by requesting the elements for a specific device through a client’s elements property.

See the HID specification for more details: https://www.usb.org/hid.

## Topics

### Structures

struct Value

Data associated with a HID element.

### Instance Properties

var client: HIDDeviceClient

The client for the device with which this element is associated.

var logicalMaximum: Int64?

The logical maximum for this element’s data.

var logicalMinimum: Int64?

The logical minimum for this element’s data.

var parentCollection: HIDElementCollection

The HIDElementCollection that contains this element.

var physicalMaximum: Int64?

The physical maximum for this element’s data.

var physicalMinimum: Int64?

The physical minimum for this element’s data.

var reportID: HIDReportID?

The report ID for the report that contains this element.

var reportSize: UInt32

The size in bits of the data for this element.

var type: HIDReportType

The type of this element.

var unit: UInt32?

The HID specification compliant unit code for this element.

var unitExponent: Int8?

The calculated exponent for this element.

var usage: HIDUsage

The HID specification compliant usage for this element.

### Default Implementations

CustomStringConvertible Implementations

Equatable Implementations

Hashable Implementations

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Equatable
- Hashable
- Sendable

## See Also

### Interaction

Communicating with human interface devices

Interact with and obtain data from devices such as keyboards and mice.

actor HIDDeviceClient

A client of a physical or virtual HID compatible peripheral.

struct HIDElementCollection

A collection of items from a report descriptor for a HID device.

struct Value

Data associated with a HID element.

protocol HIDElementUpdate

A base protocol for element update types.

enum HIDReportType

Types for HID reports.

struct HIDReportID

A type to represent the report IDs of HID reports.

enum HIDUsage

A type to represent HID usage pages.

enum HIDDeviceError

Errors that the framework can throw.

enum HIDDeviceTransport

Common transport types that transmit data to or from a HID device.

enum HIDDeviceLocalizationCode

The localization codes that some HID devices declare to specify conformance to a certain format or language.

