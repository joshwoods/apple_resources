

- SMS and Call Reporting
-  ILMessageFilterAction 

Enumeration

# ILMessageFilterAction

Responds to a received message with a filter action.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+visionOS 1.0+

``` source
enum ILMessageFilterAction
```

## Topics

### Filter Actions

case none

Allows the system to show the message unfiltered due to insufficient information to determine an action.

case allow

Allows the system to show the message unfiltered.

case junk

Prevents the system from showing the message normally, filtered as a Junk message.

case promotion

Prevents the system from showing the message normally, filtered as a Promotional message.

case transaction

Prevents the system from showing the message normally, filtered as a Transactional message.

### Deprecations

static var filter: ILMessageFilterAction

Prevents the system from showing the message unfiltered.

Deprecated

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

class ILMessageFilterQueryResponse

A response to a message filter query request.

class ILNetworkResponse

A response to an HTTPS network request performed on behalf of a Message Filter app extension.

