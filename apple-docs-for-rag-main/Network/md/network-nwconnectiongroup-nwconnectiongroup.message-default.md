

- Network
- NWConnectionGroup
- NWConnectionGroup.Message
-  default 

Type Property

# default

A static object you use to send a message with default properties.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static let `default`: NWConnectionGroup.Message
```

## See Also

### Sending Messages

init(identifier: String, expiration: UInt64, priority: Double, isFinal: Bool, antecedent: NWConnection.ContentContext?, metadata: [NWProtocolMetadata]?)

Initializes a custom message context you use to send data.

