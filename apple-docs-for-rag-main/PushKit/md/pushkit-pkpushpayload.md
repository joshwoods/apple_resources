

- PushKit
-  PKPushPayload 

Class

# PKPushPayload

An object that contains information about a received PushKit notification.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.15+visionOS 1.0+watchOS 6.0+

``` source
class PKPushPayload
```

## Topics

### Payload Data

var dictionaryPayload: [AnyHashable : Any]

The contents of the received payload.

var type: PKPushType

The type value indicating how to interpret the payload.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

