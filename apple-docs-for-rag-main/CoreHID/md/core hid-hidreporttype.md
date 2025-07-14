

- Core HID
-  HIDReportType 

Enumeration

# HIDReportType

Types for HID reports.

macOS 15.0+

``` source
enum HIDReportType
```

## Overview

For more details, see Human Interface Devices (HID) Specifications and Tools.

## Topics

### Operators

static func == (HIDReportType, HIDReportType) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case feature

A feature report is bidirectional configuration data, typically used to alter device or software functionality.

case input

An input report is data dispatched from the device to the system, typically sent in response to human interaction with one of the device controls.

case output

An output report is data sent from the system to the device, typically used to set a device control.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Interaction

Communicating with human interface devices

Interact with and obtain data from devices such as keyboards and mice.

actor HIDDeviceClient

A client of a physical or virtual HID compatible peripheral.

struct HIDElement

A representation of an item from a report descriptor for a HID device.

struct HIDElementCollection

A collection of items from a report descriptor for a HID device.

struct Value

Data associated with a HID element.

protocol HIDElementUpdate

A base protocol for element update types.

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

