

- Core HID
- HIDElement
-  HIDElement.Value 

Structure

# HIDElement.Value

Data associated with a HID element.

macOS 15.0+

``` source
struct Value
```

## Mentioned in 

Communicating with human interface devices

## Overview

Elements can have data associated with them. This data could be received as an update from the device to indicate user interaction, or could be provided to the device to alter functionality, such as turning on an LED. As the data for an element could be constantly changing, values should be seen as a snapshot of the element’s data at a specific time, and not valid at any other times.

Element values can be received by a HIDDeviceClient using HIDDeviceClient.Notification.elementUpdates(values:) after the device issues an input report, or requested from the device by providing a HIDDeviceClient.RequestElementUpdate to updateElements(_:timeout:). Element values can be sent to a device by providing a HIDDeviceClient.ProvideElementUpdate to updateElements(_:timeout:).

## Topics

### Create a HID element from a value

init(element: HIDElement, fromBytes: Data, timestamp: SuspendingClock.Instant)

Creates a value for an HID element.

init?&lt;FloatingPointType>(element: HIDElement, fromPhysicalValue: FloatingPointType, timestamp: SuspendingClock.Instant)

Creates a HID element value from a physical value.

init?&lt;IntegerType>(element: HIDElement, fromLogicalValueTruncatingIfNeeded: IntegerType, timestamp: SuspendingClock.Instant)

Creates a HID element value from a logical value.

init&lt;IntegerType>(element: HIDElement, fromIntegerTruncatingIfNeeded: IntegerType, timestamp: SuspendingClock.Instant)

Creates an HID element value from an integer.

var element: HIDElement

The HIDElement associated with this value.

### Get element data and values

var bytes: Data

The data as an array of bytes.

func integerValue&lt;IntegerType>(asTypeTruncatingIfNeeded: IntegerType.Type) -> IntegerType

The raw value of the data cast as an integer type, with no transformations applied.

func logicalValue&lt;IntegerType>(asTypeTruncatingIfNeeded: IntegerType.Type) -> IntegerType?

The raw value of the data cast as an integer type and bound by the HIDElement’s logical minimum and logical maximum values.

func physicalValue&lt;IntegerType, FloatingType>(fromTypeTruncatingIfNeeded: IntegerType.Type, as: FloatingType.Type) -> FloatingType?

The logical value of the data, shifted and scaled by the HIDElement’s physical minimum, physical maximum and exponent.

var timestamp: SuspendingClock.Instant

The time that this data was received by the system.

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

struct HIDElement

A representation of an item from a report descriptor for a HID device.

struct HIDElementCollection

A collection of items from a report descriptor for a HID device.

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

