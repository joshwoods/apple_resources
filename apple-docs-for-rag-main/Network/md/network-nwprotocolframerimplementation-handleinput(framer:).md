

- Network
- NWProtocolFramerImplementation
-  handleInput(framer:) 

Instance Method

# handleInput(framer:)

Notifies your protocol that new inbound data is available to parse.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func handleInput(framer: NWProtocolFramer.Instance) -> Int
```

**Required**

## See Also

### Handling Data

func handleOutput(framer: NWProtocolFramer.Instance, message: NWProtocolFramer.Message, messageLength: Int, isComplete: Bool)

Notifies your protocol about a new outbound message.

**Required**

