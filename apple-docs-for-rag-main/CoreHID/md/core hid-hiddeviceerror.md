

- Core HID
-  HIDDeviceError 

Enumeration

# HIDDeviceError

Errors that the framework can throw.

macOS 15.0+

``` source
enum HIDDeviceError
```

## Topics

### Operators

static func == (HIDDeviceError, HIDDeviceError) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case aborted

The request was aborted.

case badArgument

The request contains an inappropriate argument.

case busy

The device is busy.

case deviceError

There was an error with the device that couldn’t be further determined.

case exclusiveAccess

Another client posesses exclusive access to this device.

case ioError

An input/output error occurred between the host and the device.

case messageTooLarge

The data provided to a function was too large for the device to handle.

case noPower

The device isn’t powered.

case noResources

The device doesn’t have the resources required to handle this request.

case notPermitted

The client isn’t permitted to make this request with the provided arguments.

case notPrivileged

The client doesn’t have the privileges required to make this request.

case notReady

The device isn’t ready for this request.

case notResponding

The device isn’t responding.

case timeout

The request timed out.

case unknown(Int32)

A catch-all for uncommon errors.

case unsupported

The request with the provided arguments isn’t supported.

### Instance Properties

var errorDescription: String?

A localized message describing what error occurred.

### Default Implementations

Equatable Implementations

Error Implementations

LocalizedError Implementations

## Relationships

### Conforms To

- Equatable
- Error
- LocalizedError
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

enum HIDDeviceTransport

Common transport types that transmit data to or from a HID device.

enum HIDDeviceLocalizationCode

The localization codes that some HID devices declare to specify conformance to a certain format or language.

