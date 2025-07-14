

- Core HID
- HIDUsage
-  HIDUsage.SOCUsage 

Enumeration

# HIDUsage.SOCUsage

macOS 15.0+

``` source
enum SOCUsage
```

## Topics

### Enumeration Cases

case fileOffsetInBytes

case filePayload

case filePayloadContainsLastBytes

case filePayloadSizeInBytes

case fileTransferSizeMaxInBytes

case fileTransferStop

case fileTransferTillEnd

case firmwareFileId

case firmwareTransfer

case socControl

### Initializers

init?(rawValue: UInt16)

Creates a new instance with the specified raw value.

### Instance Properties

var rawValue: UInt16

The corresponding value of the raw type.

### Type Aliases

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Type Properties

static let page: UInt16

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

