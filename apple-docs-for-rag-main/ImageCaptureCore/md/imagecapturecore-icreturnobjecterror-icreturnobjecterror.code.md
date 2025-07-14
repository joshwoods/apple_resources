

- ImageCaptureCore
- ICReturnObjectError
-  ICReturnObjectError.Code 

Enumeration

# ICReturnObjectError.Code

iOSiPadOSMac CatalystmacOSvisionOS

``` source
enum Code
```

## Topics

### Enumeration Cases

case codeObjectCouldNotBeRead

The object could not be read.

case codeObjectDataEmpty

The object data is empty.

case codeObjectDataOffsetInvalid

The object data offset is invalid.

case codeObjectDataRequestTooLarge

case codeObjectDoesNotExist

The object does not exist.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Error Codes

static var codeObjectDoesNotExist: ICReturnObjectError.Code

The object does not exist.

static var codeObjectDataOffsetInvalid: ICReturnObjectError.Code

The object data offset is invalid.

static var codeObjectCouldNotBeRead: ICReturnObjectError.Code

The object could not be read.

static var codeObjectDataEmpty: ICReturnObjectError.Code

The object data is empty.

