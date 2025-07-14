

- SMS and Call Reporting
-  ILMessageFilterQueryResponse 

Class

# ILMessageFilterQueryResponse

A response to a message filter query request.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+visionOS 1.0+

``` source
class ILMessageFilterQueryResponse
```

## Topics

### Specifying the Action

var action: ILMessageFilterAction

The action the Message Filter app extension recommends that the system perform on the queried message.

var subAction: ILMessageFilterSubAction

The subaction the Message Filter app extension recommends that the system perform on the queried message.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Responses

class ILNetworkResponse

A response to an HTTPS network request performed on behalf of a Message Filter app extension.

enum ILMessageFilterAction

Responds to a received message with a filter action.

