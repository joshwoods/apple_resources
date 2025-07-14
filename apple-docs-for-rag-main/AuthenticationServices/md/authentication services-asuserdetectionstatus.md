

- Authentication Services
-  ASUserDetectionStatus 

Enumeration

# ASUserDetectionStatus

Possible values for the real user indicator.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
enum ASUserDetectionStatus
```

## Topics

### User Status

case likelyReal

The user appears to be a real person.

case unknown

The system hasn’t determined whether the user might be a real person.

case unsupported

The system can’t determine this user’s status as a real person.

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

### Detecting User Characteristics

var realUserStatus: ASUserDetectionStatus

A value that indicates whether the user appears to be a real person.

