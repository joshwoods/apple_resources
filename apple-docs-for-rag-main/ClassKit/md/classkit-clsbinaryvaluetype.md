

- ClassKit
-  CLSBinaryValueType 

Enumeration

# CLSBinaryValueType

The kinds of outcomes that a binary activity item can represent.

iOS 11.3+iPadOS 11.3+Mac Catalyst 11.3+macOS 11.0+visionOS 1.0+

``` source
enum CLSBinaryValueType
```

## Topics

### Value Types

case passFail

Pass or fail.

case trueFalse

True or false.

case yesNo

Yes or no.

case correctIncorrect

Correct or incorrect.

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

### Creating Binary Activity Items

init(identifier: String, title: String, type: CLSBinaryValueType)

Initializes a new binary activity item of the given type.

