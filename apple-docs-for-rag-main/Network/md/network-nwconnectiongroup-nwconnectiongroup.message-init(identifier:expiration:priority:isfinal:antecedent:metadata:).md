

- Network
- NWConnectionGroup
- NWConnectionGroup.Message
-  init(identifier:expiration:priority:isFinal:antecedent:metadata:) 

Initializer

# init(identifier:expiration:priority:isFinal:antecedent:metadata:)

Initializes a custom message context you use to send data.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
override init(
    identifier: String,
    expiration: UInt64 = super,
    priority: Double = super,
    isFinal: Bool = super,
    antecedent: NWConnection.ContentContext? = nil,
    metadata: [NWProtocolMetadata]? = super
)
```

## See Also

### Sending Messages

static let `default`: NWConnectionGroup.Message

A static object you use to send a message with default properties.

