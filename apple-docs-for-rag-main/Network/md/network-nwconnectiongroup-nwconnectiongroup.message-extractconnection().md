

- Network
- NWConnectionGroup
- NWConnectionGroup.Message
-  extractConnection() 

Instance Method

# extractConnection()

Converts a message you receive from an endpoint into a connection object that you use for long-term communication with that endpoint.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
func extractConnection() -> NWConnection?
```

## See Also

### Replying to Received Messages

func reply(content: Data?, message: NWConnectionGroup.Message)

Sends a reply to the specific endpoint that originates a group message you receive.

