

- Foundation
- NSCoder
-  NSCoder.DecodingFailurePolicy 

Enumeration

# NSCoder.DecodingFailurePolicy

Policies describing the action the coder should take when encountering decode failures.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum DecodingFailurePolicy
```

## Topics

### Failure Policies

case raiseException

A failure policy that directs the coder to raise an exception.

case setErrorAndReturn

A failure policy that directs the coder to capture the failure as an error object.

case raiseException

A failure policy that directs the coder to raise an exception.

case setErrorAndReturn

A failure policy that directs the coder to capture the failure as an error object.

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

### Inspecting a Coder

var allowsKeyedCoding: Bool

A Boolean value that indicates whether the receiver supports keyed coding of objects.

func containsValue(forKey: String) -> Bool

Returns a Boolean value that indicates whether an encoded value is available for a string.

var decodingFailurePolicy: NSCoder.DecodingFailurePolicy

The action the coder should take when decoding fails.

