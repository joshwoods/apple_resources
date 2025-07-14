

- Core Foundation
-  CFPropertyListFormat 

Enumeration

# CFPropertyListFormat

Specifies the format of a property list.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum CFPropertyListFormat
```

## Topics

### Constants

case openStepFormat

OpenStep format (use of this format is discouraged).

case xmlFormat_v1_0

XML format version 1.0.

case binaryFormat_v1_0

Binary format version 1.0.

### Initializers

init?(rawValue: CFIndex)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

Property List Mutability Options

Option flags that determine the degree of mutability of newly created property lists.

Reading and Writing Error Codes

Error codes for property list reading and writing functions such as CFPropertyListCreateWithData(_:_:_:_:_:).

