

- Core HID
-  HIDReportID 

Structure

# HIDReportID

A type to represent the report IDs of HID reports.

macOS 15.0+

``` source
struct HIDReportID
```

## Mentioned in 

Communicating with human interface devices

## Overview

Report IDs are defined to be 1 byte in the HID specification, and can help identify the reports received from or sent to a device. Report IDs are optional. If a descriptor only has one report, a report ID is unnecessary. A report ID of 0 is invalid.

For more details, see Human Interface Devices (HID) Specifications and Tools.

## Topics

### Operators

static func &lt; (HIDReportID, HIDReportID) -> Bool

Returns a Boolean value indicating whether the value of the first argument is less than that of the second argument.

### Initializers

init?(rawValue: UInt8)

Creates a HID report ID.

### Instance Properties

var rawValue: HIDReportID.RawValue

The raw value of the report ID.

### Type Aliases

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Type Properties

static let allReports: ClosedRange&lt;HIDReportID>

A convenient definition that represents every possible report ID.

### Default Implementations

Comparable Implementations

CustomStringConvertible Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- Comparable
- Copyable
- CustomStringConvertible
- Equatable
- Hashable
- RawRepresentable
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

enum HIDReportType

Types for HID reports.

enum HIDUsage

A type to represent HID usage pages.

enum HIDDeviceError

Errors that the framework can throw.

enum HIDDeviceTransport

Common transport types that transmit data to or from a HID device.

enum HIDDeviceLocalizationCode

The localization codes that some HID devices declare to specify conformance to a certain format or language.

