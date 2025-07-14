

- Core HID
-  HIDElementUpdate 

Protocol

# HIDElementUpdate

A base protocol for element update types.

macOS 15.0+

``` source
protocol HIDElementUpdate : Hashable, Sendable
```

## Overview

Not intended to be used directly, see HIDDeviceClient.ProvideElementUpdate and HIDDeviceClient.RequestElementUpdate.

## Relationships

### Inherits From

- Equatable
- Hashable
- Sendable

### Conforming Types

- HIDDeviceClient.ProvideElementUpdate
- HIDDeviceClient.RequestElementUpdate

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

