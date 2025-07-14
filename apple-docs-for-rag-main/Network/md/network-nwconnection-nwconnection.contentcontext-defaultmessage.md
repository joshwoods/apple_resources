

- Network
- NWConnection
- NWConnection.ContentContext
-  defaultMessage 

Type Property

# defaultMessage

A static context representing a message with default properties.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
static let defaultMessage: NWConnection.ContentContext
```

## Discussion

You should use this context for sending content unless there is a reason to override some values.

## See Also

### Using Constant Send Contexts

static let finalMessage: NWConnection.ContentContext

A static context that’s marked as the final message in a connection.

static let defaultStream: NWConnection.ContentContext

A static context representing the total stream of bytes on a connection.

