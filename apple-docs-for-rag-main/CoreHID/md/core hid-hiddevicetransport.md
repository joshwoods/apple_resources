

- Core HID
-  HIDDeviceTransport 

Enumeration

# HIDDeviceTransport

Common transport types that transmit data to or from a HID device.

macOS 15.0+

``` source
enum HIDDeviceTransport
```

## Overview

If a device declares an uncommon transport, the HIDDeviceTransport.unknown(_:) case is used with the associated raw string value.

## Topics

### Operators

static func == (HIDDeviceTransport, HIDDeviceTransport) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case aid

case airPlay

case bluetooth

case bluetoothAACP

case bluetoothLowEnergy

case fifo

case i2c

case iap

case serial

case spi

case spu

case unknown(String)

case usb

case virtual

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
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

struct HIDReportID

A type to represent the report IDs of HID reports.

enum HIDUsage

A type to represent HID usage pages.

enum HIDDeviceError

Errors that the framework can throw.

enum HIDDeviceLocalizationCode

The localization codes that some HID devices declare to specify conformance to a certain format or language.

