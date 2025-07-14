

- SMS and Call Reporting
-  ILClassificationAction 

Enumeration

# ILClassificationAction

The actions the system can take in response to the reported communication.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+visionOS 1.0+

``` source
enum ILClassificationAction
```

## Topics

### Classifications

case none

No action is required.

case reportJunk

The system should report the communication as junk.

case reportJunkAndBlockSender

The system should report the communication as junk and add the number to the system’s block list.

case reportNotJunk

The system should report that the communication is not junk.

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

### Responses

class ILClassificationResponse

A response object that tells the system how to handle the reported communications.

